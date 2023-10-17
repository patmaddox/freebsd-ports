PORTNAME=	minimal-snowplow-tracker
PORTVERSION=	0.0.2
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	A minimal snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
WWW=		https://pypi.org/project/minimal-snowplow-tracker/

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	autoplist concurrent distutils

RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}requests>0:www/py-requests@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}six>0:devel/py-six@${PY_FLAVOR}

.include <bsd.port.mk>
