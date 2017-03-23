# New ports collection makefile for: FreeBSD settings for grub2
# Date created:        29 jun 2015
# Whom:                angelescuo@yahoo.com
#
# $FreeBSD$
#

PORTNAME=	freebsd-grub2-settings
PORTVERSION=	1.0
CATEGORIES=	sysutils

MAINTAINER=	angelescuo@yahoo.com
COMMENT=	FreeBSD grub2 settings

LICENSE=	BSD

USE_GITHUB=	yes
GH_ACCOUNT=	wallisonalves

NO_BUILD=	yes

RUN_DEPENDS=	grub-mkconfig:sysutils/grub2-pcbsd

do-install:
	${MKDIR} ${STAGEDIR}/boot/grub/themes/freebsd
	${MKDIR} ${STAGEDIR}/usr/local/etc/default
	${CP} -R  ${WRKSRC}/* ${STAGEDIR}/
.include <bsd.port.mk>
