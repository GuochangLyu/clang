set(LLVM_LINK_COMPONENTS Support)

add_tablegen(clang-tblgen CLANG
  ClangASTNodesEmitter.cpp
  ClangAttrEmitter.cpp
  ClangCommentCommandInfoEmitter.cpp
  ClangCommentHTMLNamedCharacterReferenceEmitter.cpp
  ClangCommentHTMLTagsEmitter.cpp
  ClangDataCollectorsEmitter.cpp
  ClangDiagnosticsEmitter.cpp
  ClangOpcodesEmitter.cpp
  ClangOpenCLBuiltinEmitter.cpp
  ClangOptionDocEmitter.cpp
  ClangSACheckersEmitter.cpp
  ClangTypeNodesEmitter.cpp
  NeonEmitter.cpp
  TableGen.cpp
  )
set_target_properties(clang-tblgen PROPERTIES FOLDER "Clang tablegenning")
