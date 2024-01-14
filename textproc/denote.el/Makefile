PORTNAME=	denote.el
PORTVERSION=	2.2.0
CATEGORIES=	textproc

MAINTAINER=	pat@patmaddox.com
COMMENT=	Simple notes with an efficient file-naming scheme for Emacs
WWW=		https://protesilaos.com/emacs/denote

LICENSE=	GPLv3

USES=			emacs
EMACS_NO_DEPENDS=	yes

USE_GITHUB=	yes
GH_ACCOUNT=	protesilaos
GH_PROJECT=	denote

NO_ARCH=	yes
NO_BUILD=	yes

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}
	${INSTALL_DATA} ${WRKSRC}/*.el ${STAGEDIR}${PREFIX}/${EMACS_SITE_LISPDIR}

.include <bsd.port.mk>
