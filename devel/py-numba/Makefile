# $FreeBSD: $ 

PORTNAME=	numba
PORTVERSION=	0.27.0
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dave@dal.ca
COMMENT=	Numba is an optimizing compiler for Python, using LLVM 

LICENSE=	BSD

USES=		fortran python
USE_PYTHON=	distutils autoplist

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}llvmlite>0:${PORTSDIR}/devel/py-llvmlite \
		${PYTHON_PKGNAMEPREFIX}numpy>0:${PORTSDIR}/math/py-numpy \
		${PYTHON_PKGNAMEPREFIX}funcsigs>0:${PORTSDIR}/devel/py-funcsigs

.include <bsd.port.mk>
