include $(THEOS)/makefiles/common.mk

TWEAK_NAME = VideoDownloaderCN
VideoDownloaderCN_FILES = WeChatMomentVideo.xm WeiboVideo.xm Neteasemusic.xm TwitterVideo.xm BaiduTB.xm QQVideo.xm articleNews.xm QQMusic.xm YouTubeVideo.xm lib/MBProgressHUD/MBProgressHUD.m lib/DownloaderManager/DownloaderManager.m lib/VideoAudioComposition/VideoAudioComposition.m

VideoDownloaderCN_CFLAGS = -fobjc-arc

export ARCHS = armv7 armv7s arm64 arm64e
export TARGET = iphone:clang:12.2:8.0

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	# install.exec "killall -9 SpringBoard"
SUBPROJECTS += videodownloadercnprefs
include $(THEOS_MAKE_PATH)/aggregate.mk
