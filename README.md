# toolset

watchexec \
  -c clear \
  -o do-nothing \
  -d 100ms \
  --exts go \
  'pkg=".${WATCHEXEC_COMMON_PATH/$PWD/}/..."; echo "running tests for $pkg"; go test "$pkg"'
