PORTNAME=	setuptools_dso
PORTVERSION=	2.9
CATEGORIES=	devel
MASTER_SITES=	PYPI

MAINTAINER=	pat@patmaddox.com
COMMENT=	setuptools extension to build non-python shared libraries
WWW=		https://github.com/mdavidsaver/setuptools_dso

LICENSE=	BSD

USES=		python
USE_PYTHON=	autoplist concurrent distutils

#RUN_DEPENDS+= 	${PYTHONPREFIX_SITELIBDIR}/agate:textproc/py-agate@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/click:devel/py-click@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/dateutil:devel/py-dateutil@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/logbook:devel/py-logbook@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/snowplow_tracker:devel/py-minimal-snowplow-tracker@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/pytz:devel/py-pytz@${PY_FLAVOR} \
#	${PYTHONPREFIX_SITELIBDIR}/requests:www/py-requests@${PY_FLAVOR} \

#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}
#RUN_DEPENDS+=	${PYTHON_PKGNAMEPREFIX}click:devel/py-click@${PY_FLAVOR} ${PYTHON_PKGNAMEPREFIX}logbook:devel/py-logbook@${PY_FLAVOR}

.include <bsd.port.mk>
