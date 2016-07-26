# Created by David Kalliecharan <dave@dal.ca>
# $FreeBSD$

PORTNAME=	numba
PORTVERSION=	0.27.0
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dave@dal.ca
COMMENT=	Numba is an optimizing compiler for Python, using LLVM 

LICENSE=	BSD
LICENSE_FILE=	${WRKSRC}/LICENSE

# Uses Python 2.7, 3.4+
USES=		python
USE_PYTHON=	distutils autoplist

.include <bsd.port.pre.mk>

BUILD_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}numpy>1.7:${PORTSDIR}/math/py-numpy

# Requried for Python 2.7
.if ${PYTHON_REL} < 3400
RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}enum34>0:${PORTSDIR}/devel/py-enum34 \
		${PYTHON_PKGNAMEPREFIX}singledispatch>0:${PORTSDIR}/devel/py-singledispatch \
		${PYTHON_PKGNAMEPREFIX}funcsigs>0:${PORTSDIR}/devel/py-funcsigs
.endif

RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}llvmlite>=0.12:${PORTSDIR}/devel/py-llvmlite \
		${PYTHON_PKGNAMEPREFIX}argparse>0:${PORTSDIR}/devel/py-argparse

.include <bsd.port.post.mk>
