set(LLVM_LINK_COMPONENTS support)

add_clang_executable(fineParP2S
  Example.cpp
  )
target_link_libraries(fineParP2S
  clangTooling
  clangBasic
  clangASTMatchers

  clangFrontend
  clangSerialization
  clangDriver
  clangTooling
  clangParse
  clangSema
  clangAnalysis
  clangRewriteFrontend
  clangEdit
  clangAST
  clangLex
  clangBasic
  )

