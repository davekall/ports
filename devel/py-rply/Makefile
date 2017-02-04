# Created by David Kalliecharan <dave@dal.ca>
# $FreeBSD$

PORTNAME=	rply
PORTVERSION=	0.7.4
PORTREVISION=	1
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	dave@dal.ca
COMMENT=	A pure python parser generator, that also works with RPython

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		python 
USE_PYTHON=	distutils autoplist

RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}appdirs>0:devel/py-appdirs \

.include <bsd.port.mk>
