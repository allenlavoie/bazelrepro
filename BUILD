cc_library(
	name="regular_dep",
	hdrs=["regular_dep.h"],
	srcs=["regular_dep.cc"],
)

cc_binary(
	name="libsome.so",
	linkshared=1,
)

cc_test(
	name="link_repro",
	srcs=[
            "test.cc",
            ":libsome.so"
          ],
	deps=[":regular_dep"],
)
