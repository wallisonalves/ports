# New ports collection makefile for: xfce settings in installed mode
# Date created:        17 may 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	xfce-installed-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD xfce settings in installed mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

RUN_DEPENDS=	pkg:archivers/pkg

NO_BUILD=	yes

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/xfce-installed-settings/etc/skel
	${CP} -R   ${WRKSRC}/etc/skel/* ${STAGEDIR}/${PREFIX}/share/freebsd/xfce-installed-settings/etc/skel
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd/xfce-installed-settings/etc/default/grub.d
	${CP} -R   ${WRKSRC}/etc/default/* ${STAGEDIR}/${PREFIX}/share/freebsd/xfce-installed-settings/etc/default
.include <bsd.port.mk>
