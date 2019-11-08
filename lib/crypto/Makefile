# SPDX-License-Identifier: GPL-2.0

# chacha is used by the /dev/random driver which is always builtin
obj-y						+= chacha.o
obj-$(CONFIG_CRYPTO_LIB_CHACHA_GENERIC)		+= libchacha.o

obj-y += libblake2s.o
libblake2s-y += blake2s.o blake2s-generic.o
ifneq ($(CONFIG_CRYPTO_MANAGER_DISABLE_TESTS),y)
libblake2s-y += blake2s-selftest.o
endif
