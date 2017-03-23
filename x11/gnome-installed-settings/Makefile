# New ports collection makefile for: gnome settings in installed mode
# Date created:        17 may 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	gnome-installed-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD gnome settings in installed mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

RUN_DEPENDS=	pkg:archivers/pkg

NO_BUILD=	yes

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/gnome-installed-settings
	${CP} -R   ${WRKSRC}/freebsd/* ${STAGEDIR}/${PREFIX}/share/freebsd/gnome-installed-settings
.include <bsd.port.mk>
