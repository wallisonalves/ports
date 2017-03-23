# New ports collection makefile for: freebsd common settings in installed mode
# Date created:        17 may 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	freebsd-installed-common-settings
PORTVERSION=	1.0
CATEGORIES=	x11

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD common settings in installed mode

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

NO_BUILD=	yes

RUN_DEPENDS= pkg:archivers/pkg

do-install:
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/freebsd
	${CP} -R   ${WRKSRC}/freebsd/* ${STAGEDIR}/${PREFIX}/share/freebsd
	${MKDIR} -p ${STAGEDIR}/${PREFIX}/usr/local/share/freebsd/common-installed-settings/base/backup/boot
	${MKDIR} -p ${STAGEDIR}/${PREFIX}/usr/local/share/freebsd/common-installed-settings/base/backup/etc
	${MKDIR} -p ${STAGEDIR}/${PREFIX}/usr/local/share/freebsd/common-installed-settings/packages/backup/etc/X11
	${MKDIR} ${STAGEDIR}/${PREFIX}/share/sounds
	${CP} -R   ${WRKSRC}/usr/local/* ${STAGEDIR}/${PREFIX}
.include <bsd.port.mk>
