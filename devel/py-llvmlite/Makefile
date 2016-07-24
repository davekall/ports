# $FreeBSD: $ 

PORTNAME=	llvmlite
PORTVERSION=	0.12.1
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dave@dal.ca
COMMENT=	A lightweight LLVM python binding for writing JIT compilers

LICENSE=	BSD

USES=		python:2.7-3.3 
USE_PYTHON=	distutils autoplist

LLVM_VER=	37

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}enum34>0:${PORTSDIR}/devel/py-enum34 \
		llvm-config${LLVM_VER}:devel/llvm${LLVM_VER}

MAKE_ENV=	LLVM_CONFIG=${LOCALBASE}/bin/llvm-config${LLVM_VER}

.include <bsd.port.mk>
