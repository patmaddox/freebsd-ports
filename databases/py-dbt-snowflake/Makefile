PORTNAME=	dbt-snowflake
PORTVERSION=	1.6.0
CATEGORIES=	databases python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	dbt adapter for Snowflake
WWW=		https://github.com/dbt-labs/dbt-snowflake

LICENSE=	APACHE20

USES=		python
USE_PYTHON=	concurrent distutils

RUN_DEPENDS=	dbt:devel/py-dbt-core \
		${PYTHONPREFIX_SITELIBDIR}/asn1crypto/__init__.py:devel/py-asn1crypto@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/certifi/__init__.py:security/py-certifi@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/cffi/__init__.py:devel/py-cffi@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/charset_normalizer/__init__.py:textproc/py-charset-normalizer@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/cryptography/__init__.py:security/py-cryptography@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/Cryptodome/__init__.py:security/py-pycryptodomex@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/filelock/__init__.py:sysutils/py-filelock@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/importlib_metadata/__init__.py:devel/py-importlib-metadata@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/idna/__init__.py:dns/py-idna@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/jwt/__init__.py:www/py-pyjwt@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/OpenSSL/__init__.py:security/py-openssl@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/oscrypto/__init__.py:security/py-oscrypto@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/packaging/__init__.py:devel/py-packaging@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/platformdirs/__init__.py:devel/py-platformdirs@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/requests/__init__.py:www/py-requests@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/snowflake/connector/__init__.py:databases/py-snowflake-connector@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/sortedcontainers/__init__.py:devel/py-sortedcontainers@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/tomlkit/__init__.py:textproc/py-tomlkit@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/typing_extensions.py:devel/py-typing-extensions@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/pytz/__init__.py:devel/py-pytz@${PY_FLAVOR} \
		${PYTHONPREFIX_SITELIBDIR}/urllib3/__init__.py:net/py-urllib3@${PY_FLAVOR}

.include <bsd.port.mk>
