# Created by David Kalliecharan <dave@dal.ca>
# $FreeBSD$ 

PORTNAME=	llvmlite
PORTVERSION=	0.12.1
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dave@dal.ca
COMMENT=	A lightweight LLVM python binding for writing JIT compilers

LICENSE=	BSD
LICENSE_FILE=	${WRKSRC}/LICENSE

# Python 2.7,3.4+
USES=		python
USE_PYTHON=	distutils autoplist

.include <bsd.port.pre.mk>

# README claims LLVM 3.8, but 0.12.1 branch README requires LLVM 3.7.
LLVM_VER=	37

# Python 2.7 requires enum34, Python 3.4+ unecessary
.if ${PYTHON_REL} < 3400
BUILD_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}enum34>0:${PORTSDIR}/devel/py-enum34
.endif

BUILD_DEPENDS+=	llvm-config${LLVM_VER}:devel/llvm${LLVM_VER}

MAKE_ENV=	LLVM_CONFIG=${LOCALBASE}/bin/llvm-config${LLVM_VER}

.include <bsd.port.post.mk>
