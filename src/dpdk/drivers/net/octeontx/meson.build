# SPDX-License-Identifier: BSD-3-Clause
# Copyright(c) 2017 Cavium, Inc

if is_windows
	build = false
	reason = 'not supported on Windows'
	subdir_done()
endif

subdir('base')
objs = [base_objs]

sources = files('octeontx_rxtx.c',
		'octeontx_ethdev.c',
		'octeontx_ethdev_ops.c'
		)

deps += ['mempool_octeontx', 'eventdev']

includes += include_directories('base')
