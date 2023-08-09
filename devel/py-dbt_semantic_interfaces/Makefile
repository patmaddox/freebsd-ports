PORTNAME=	dbt_semantic_interfaces
PORTVERSION=	0.2.0
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	The shared semantic layer definitions that dbt-core and MetricFlow use.
WWW=		https://github.com/dbt-labs/dbt-semantic-interfaces

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent pep517

BUILD_DEPENDS+= hatch:devel/py-hatch@${PY_FLAVOR} \
		hatchling:devel/py-hatchling@${PY_FLAVOR}

.include <bsd.port.mk>
