AM_CFLAGS = -g -Wall -D_GNU_SOURCE -I$(srcdir)/include

bin_PROGRAMS = \
	simple/fi_info \
	simple/fi_msg\
	simple/fi_msg_pingpong \
	simple/fi_msg_rma \
	simple/fi_rdm \
	simple/fi_rdm_rma_simple \
	simple/fi_dgram \
	simple/fi_dgram_waitset \
	simple/fi_rdm_pingpong \
	simple/fi_rdm_tagged_pingpong \
	simple/fi_rdm_tagged_search \
	simple/fi_rdm_cntr_pingpong \
	simple/fi_rdm_rma \
	simple/fi_rdm_atomic \
	simple/fi_ud_pingpong \
	simple/fi_cq_data \
	simple/fi_poll \
	simple/fi_rdm_inject_pingpong \
	simple/fi_rdm_multi_recv \
	simple/fi_scalable_ep \
	simple/fi_rdm_shared_ctx \
	unit/fi_eq_test \
	unit/fi_av_test \
	unit/fi_size_left_test \
	unit/fi_dom_test \
	unit/fi_ep_test \
	ported/libibverbs/fi_rc_pingpong \
	ported/librdmacm/fi_cmatose \
	complex/fabtest

bin_SCRIPTS = scripts/cray_runall.sh

simple_fi_info_SOURCES = \
	simple/info.c \
	common/shared.c

simple_fi_msg_SOURCES = \
	simple/msg.c \
	common/shared.c

simple_fi_msg_pingpong_SOURCES = \
	simple/msg_pingpong.c \
	common/shared.c

simple_fi_msg_rma_SOURCES = \
	simple/msg_rma.c \
	common/shared.c

simple_fi_rdm_SOURCES = \
	simple/rdm.c \
	common/shared.c

simple_fi_rdm_rma_simple_SOURCES = \
	simple/rdm_rma_simple.c \
	common/shared.c

simple_fi_dgram_SOURCES = \
	simple/dgram.c \
	common/shared.c

simple_fi_dgram_waitset_SOURCES = \
	simple/dgram_waitset.c \
	common/shared.c

simple_fi_rdm_pingpong_SOURCES = \
	simple/rdm_pingpong.c \
	common/shared.c

simple_fi_rdm_tagged_pingpong_SOURCES = \
	simple/rdm_tagged_pingpong.c \
	common/shared.c

simple_fi_rdm_tagged_search_SOURCES = \
	simple/rdm_tagged_search.c \
	common/shared.c

simple_fi_rdm_cntr_pingpong_SOURCES = \
	simple/rdm_cntr_pingpong.c \
	common/shared.c

simple_fi_rdm_rma_SOURCES = \
	simple/rdm_rma.c \
	common/shared.c
	
simple_fi_rdm_atomic_SOURCES = \
	simple/rdm_atomic.c \
	common/shared.c

simple_fi_ud_pingpong_SOURCES = \
	simple/ud_pingpong.c \
	common/shared.c

simple_fi_cq_data_SOURCES = \
	simple/cq_data.c \
	common/shared.c

simple_fi_rdm_inject_pingpong_SOURCES = \
	simple/rdm_inject_pingpong.c \
	common/shared.c

simple_fi_scalable_ep_SOURCES = \
	simple/scalable_ep.c \
	common/shared.c

simple_fi_rdm_shared_ctx_SOURCES = \
	simple/rdm_shared_ctx.c \
	common/shared.c

simple_fi_poll_SOURCES = \
	simple/poll.c \
	common/shared.c

simple_fi_rdm_multi_recv_SOURCES = \
	simple/rdm_multi_recv.c \
	common/shared.c

unit_fi_eq_test_SOURCES = \
	unit/eq_test.c \
	unit/common.c \
	common/shared.c

unit_fi_av_test_SOURCES = \
	unit/av_test.c \
	unit/common.c

unit_fi_dom_test_SOURCES = \
	unit/dom_test.c \
	unit/common.c

unit_fi_ep_test_SOURCES = \
	unit/ep_test.c \
	unit/common.c

unit_fi_size_left_test_SOURCES = \
	unit/size_left_test.c \
	unit/common.c

ported_libibverbs_fi_rc_pingpong_SOURCES = \
	ported/libibverbs/rc_pingpong.c

ported_librdmacm_fi_cmatose_SOURCES = \
	ported/librdmacm/cmatose.c

complex_fabtest_SOURCES = \
	complex/fabtest.c \
	complex/ft_comm.c \
	complex/ft_comp.c \
	complex/ft_config.c \
	complex/ft_domain.c \
	complex/ft_endpoint.c \
	complex/ft_msg.c \
	complex/ft_test.c \
	common/shared.c

man_MANS = man/fabtests.7

EXTRA_DIST = \
	include/shared.h \
	include/unit_common.h \
	complex/fabtest.h \
	fabtests.spec.in $(man_MANS)

dist-hook: fabtests.spec
	cp fabtests.spec $(distdir)
