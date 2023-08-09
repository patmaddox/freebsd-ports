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

#RUN_DEPENDS+= ${PYTHONPREFIX_SITELIBDIR}/click:devel/py-click@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/logbook:devel/py-logbook@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pytz:devel/py-pytz@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/requests:www/py-requests@${PY_FLAVOR}

#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}
#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}

.include <bsd.port.mk>
