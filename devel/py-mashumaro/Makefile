PORTNAME=	mashumaro
PORTVERSION=	3.9
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	Fast and well tested serialization library on top of dataclasses
WWW=		https://github.com/Fatal1ty/mashumaro

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}typing-extensions>0:devel/py-typing-extensions@${PY_FLAVOR}

.include <bsd.port.mk>
