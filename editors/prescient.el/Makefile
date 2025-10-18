PORTNAME=	prescient.el
DISTVERSIONPREFIX=	v
DISTVERSION=	6.3.2
CATEGORIES=	editors elisp
PKGNAMESUFFIX=	${EMACS_PKGNAMESUFFIX}

MAINTAINER=	pat@patmaddox.com
COMMENT=	Simple but effective candidate sorting and filtering for Emacs
WWW=		https://github.com/radian-software/prescient.el

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.md

USES=		emacs

USE_GITHUB=	yes
GH_ACCOUNT=	radian-software

NO_ARCH=	yes
NO_BUILD=	yes

OPTIONS_DEFINE=	DOCS

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}/prescient
	${INSTALL_DATA} ${WRKSRC}/*.el ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}/prescient

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/README.md ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
