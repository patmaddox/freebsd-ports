PORTNAME=	hologram
PORTVERSION=	0.0.16
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	A library for automatically generating Draft 7 JSON Schemas from Python dataclasses
WWW=		https://github.com/dbt-labs/hologram

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}dateutil>0:devel/py-dateutil@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}jsonschema>0:devel/py-jsonschema@${PY_FLAVOR}

.include <bsd.port.mk>
