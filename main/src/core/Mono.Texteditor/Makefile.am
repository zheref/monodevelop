
ADDIN_BUILD = $(top_builddir)/build/bin
ASSEMBLY = $(top_builddir)/build/bin/Mono.TextEditor.dll
REFS =  \
	$(GLIB_SHARP_LIBS) \
	$(GTK_SHARP_LIBS) \
	-r:../../../build/bin/ICSharpCode.NRefactory.dll \
	-r:Mono.Cairo \
	-r:Mono.Posix \
	-r:System \
	-r:System.Core \
	-r:System.Drawing \
	-r:System.Xml

CONFIG=Mono.TextEditor.dll.config

FILES =  \
	AssemblyInfo.cs \
	gtk-gui/generated.cs \
	Mono.TextEditor.Highlighting.Regex/Regex.cs \
	Mono.TextEditor.Highlighting.Regex/RegexMatch.cs \
	Mono.TextEditor.Highlighting/Chunk.cs \
	Mono.TextEditor.Highlighting/ChunkStyle.cs \
	Mono.TextEditor.Highlighting/CloneableStack.cs \
	Mono.TextEditor.Highlighting/ColorScheme.cs \
	Mono.TextEditor.Highlighting/DefaultStyle.cs \
	Mono.TextEditor.Highlighting/HighlightingPartitioner.cs \
	Mono.TextEditor.Highlighting/ISyntaxMode.cs \
	Mono.TextEditor.Highlighting/IXmlProvider.cs \
	Mono.TextEditor.Highlighting/JaySyntaxMode.cs \
	Mono.TextEditor.Highlighting/Keywords.cs \
	Mono.TextEditor.Highlighting/Marker.cs \
	Mono.TextEditor.Highlighting/Match.cs \
	Mono.TextEditor.Highlighting/ReferencedChunkStyle.cs \
	Mono.TextEditor.Highlighting/Rule.cs \
	Mono.TextEditor.Highlighting/SemanticRule.cs \
	Mono.TextEditor.Highlighting/Span.cs \
	Mono.TextEditor.Highlighting/SyntaxMode.cs \
	Mono.TextEditor.Highlighting/SyntaxModeService.cs \
	Mono.TextEditor.Highlighting/XmlReadHelper.cs \
	Mono.TextEditor.PopupWindow/IListDataProvider.cs \
	Mono.TextEditor.PopupWindow/ListWidget.cs \
	Mono.TextEditor.PopupWindow/ListWindow.cs \
	Mono.TextEditor.PopupWindow/ModeHelpWindow.cs \
	Mono.TextEditor.PopupWindow/TooltipWindow.cs \
	Mono.TextEditor.Theatrics/Actor.cs \
	Mono.TextEditor.Theatrics/AnimatedBox.cs \
	Mono.TextEditor.Theatrics/AnimatedVBox.cs \
	Mono.TextEditor.Theatrics/AnimatedWidget.cs \
	Mono.TextEditor.Theatrics/Animation.cs \
	Mono.TextEditor.Theatrics/BounceFadePopupWindow.cs \
	Mono.TextEditor.Theatrics/Choreographer.cs \
	Mono.TextEditor.Theatrics/Pulsator.cs \
	Mono.TextEditor.Theatrics/SingleActorStage.cs \
	Mono.TextEditor.Theatrics/SmartScrolledWindow.cs \
	Mono.TextEditor.Theatrics/Stage.cs \
	Mono.TextEditor.Utils/Diff.cs \
	Mono.TextEditor.Utils/RedBlackTree.cs \
	Mono.TextEditor.Utils/RtfWriter.cs \
	Mono.TextEditor.Utils/TextBreaker.cs \
	Mono.TextEditor.Utils/TextFileUtility.cs \
	Mono.TextEditor.Vi/ViActionMaps.cs \
	Mono.TextEditor.Vi/ViActions.cs \
	Mono.TextEditor.Vi/ViBuilderContext.cs \
	Mono.TextEditor.Vi/ViBuilders.cs \
	Mono.TextEditor.Vi/ViCommandMap.cs \
	Mono.TextEditor.Vi/ViEditor.cs \
	Mono.TextEditor.Vi/ViEditorActions.cs \
	Mono.TextEditor.Vi/ViKeyNotation.cs \
	Mono.TextEditor.Vi/ViMacro.cs \
	Mono.TextEditor.Vi/ViMark.cs \
	Mono.TextEditor.Vi/ViMode.cs \
	Mono.TextEditor.Vi/ViWordFindStrategy.cs \
	Mono.TextEditor/Actions/BookmarkActions.cs \
	Mono.TextEditor/Actions/CaretMoveActions.cs \
	Mono.TextEditor/Actions/ClipboardActions.cs \
	Mono.TextEditor/Actions/DeleteActions.cs \
	Mono.TextEditor/Actions/FoldActions.cs \
	Mono.TextEditor/Actions/MiscActions.cs \
	Mono.TextEditor/Actions/ScrollActions.cs \
	Mono.TextEditor/Actions/SelectionActions.cs \
	Mono.TextEditor/Annotatable.cs \
	Mono.TextEditor/BookmarkMarker.cs \
	Mono.TextEditor/Caret.cs \
	Mono.TextEditor/Document/BufferedTextReader.cs \
	Mono.TextEditor/Document/DocumentChangeEventArgs.cs \
	Mono.TextEditor/Document/DocumentLine.cs \
	Mono.TextEditor/Document/DocumentLocation.cs \
	Mono.TextEditor/Document/DocumentRegion.cs \
	Mono.TextEditor/Document/DocumentUpdateRequest.cs \
	Mono.TextEditor/Document/EmacsWordFindStrategy.cs \
	Mono.TextEditor/Document/FoldingType.cs \
	Mono.TextEditor/Document/FoldSegment.cs \
	Mono.TextEditor/Document/GapBuffer.cs \
	Mono.TextEditor/Document/IBuffer.cs \
	Mono.TextEditor/Document/ILineSplitter.cs \
	Mono.TextEditor/Document/IWordFindStrategy.cs \
	Mono.TextEditor/Document/LineEventArgs.cs \
	Mono.TextEditor/Document/LineSplitter.cs \
	Mono.TextEditor/Document/PrimitiveLineSplitter.cs \
	Mono.TextEditor/Document/SegmentTree.cs \
	Mono.TextEditor/Document/SharpDevelopWordFindStrategy.cs \
	Mono.TextEditor/Document/StringBuffer.cs \
	Mono.TextEditor/Document/SyntaxModeChangeEventArgs.cs \
	Mono.TextEditor/Document/TextDocument.cs \
	Mono.TextEditor/Document/TextSegment.cs \
	Mono.TextEditor/EditMode.cs \
	Mono.TextEditor/Gui/CodeSegmentEditorWindow.cs \
	Mono.TextEditor/Gui/CodeSegmentPreviewWindow.cs \
	Mono.TextEditor/Gui/DashedLineMargin.cs \
	Mono.TextEditor/Gui/FoldingScreenbackgroundRenderer.cs \
	Mono.TextEditor/Gui/FoldMarkerMargin.cs \
	Mono.TextEditor/Gui/GtkGestures.cs \
	Mono.TextEditor/Gui/GtkWorkarounds.cs \
	Mono.TextEditor/Gui/GutterMargin.cs \
	Mono.TextEditor/Gui/HslColor.cs \
	Mono.TextEditor/Gui/IAnimationDrawer.cs \
	Mono.TextEditor/Gui/IBackgroundRenderer.cs \
	Mono.TextEditor/Gui/IconMargin.cs \
	Mono.TextEditor/Gui/ITooltipProvider.cs \
	Mono.TextEditor/Gui/Margin.cs \
	Mono.TextEditor/Gui/MarginDrawer.cs \
	Mono.TextEditor/Gui/PangoUtil.cs \
	Mono.TextEditor/Gui/TextEditor.cs \
	Mono.TextEditor/Gui/TextEditorAccessibility.cs \
	Mono.TextEditor/Gui/TextEditorContainer.cs \
	Mono.TextEditor/Gui/TextViewMargin.cs \
	Mono.TextEditor/HeightTree.cs \
	Mono.TextEditor/HelperMethods.cs \
	Mono.TextEditor/IBracketMatcher.cs \
	Mono.TextEditor/IIndentationTracker.cs \
	Mono.TextEditor/IndentStyle.cs \
	Mono.TextEditor/InsertionCursorEditMode.cs \
	Mono.TextEditor/ISearchEngine.cs \
	Mono.TextEditor/ITextEditorOptions.cs \
	Mono.TextEditor/LinkEventArgs.cs \
	Mono.TextEditor/Platform.cs \
	Mono.TextEditor/SearchRequest.cs \
	Mono.TextEditor/SearchResult.cs \
	Mono.TextEditor/Selection.cs \
	Mono.TextEditor/SimpleEditMode.cs \
	Mono.TextEditor/Standalone/IDocument.cs \
	Mono.TextEditor/Standalone/IDocumentLine.cs \
	Mono.TextEditor/Standalone/ISegment.cs \
	Mono.TextEditor/Standalone/ITextAnchor.cs \
	Mono.TextEditor/Standalone/ITextSource.cs \
	Mono.TextEditor/Standalone/TextChangeEventArgs.cs \
	Mono.TextEditor/Standalone/TextLocation.cs \
	Mono.TextEditor/Standalone/TextSourceVersionProvider.cs \
	Mono.TextEditor/TextEditorData.cs \
	Mono.TextEditor/TextEditorOptions.cs \
	Mono.TextEditor/TextLinkEditMode.cs \
	Mono.TextEditor/TextMarker.cs \
	Mono.TextEditor/TextMarkerEvent.cs 
	Mono.TextEditor.Highlighting/Match.cs \
	Mono.TextEditor.Highlighting/Style.cs \
	Mono.TextEditor.Highlighting/SyntaxMode.cs \
	Mono.TextEditor.Highlighting/XmlReadHelper.cs \
	Mono.TextEditor.Highlighting/ChunkStyle.cs \
	Mono.TextEditor.Highlighting/SyntaxModeService.cs \
	Mono.TextEditor.Highlighting/Span.cs \
	Mono.TextEditor.Tests/Mono.TextEditor.Tests.DefaultEditActions/InsertNewLineTests.cs \
	Mono.TextEditor.Tests/Mono.TextEditor.Tests.DefaultEditActions/CaretMoveTests.cs

RES =  \
	gtk-gui/gui.stetic \
	Styles/BrownStyle.xml \
	Styles/C64Style.xml \
	Styles/DefaultStyle.xml \
	Styles/GeditStyle.xml \
	Styles/IrBlackStyle.xml \
	Styles/OblivionStyle.xml \
	Styles/SolarizedDarkStyle.xml \
	Styles/SolarizedLightStyle.xml \
	Styles/Styles.xsd \
	Styles/TangoLightStyle.xml \
	Styles/VisualStudioStyle.xml \
	SyntaxModes/ActionScriptSyntaxMode.xml \
	SyntaxModes/AspNetSyntaxMode.xml \
	SyntaxModes/BooSyntaxMode.xml \
	SyntaxModes/CGSyntaxMode.xml \
	SyntaxModes/ChangeLogSyntaxMode.xml \
	SyntaxModes/CPPSyntaxMode.xml \
	SyntaxModes/CSharpSyntaxMode.xml \
	SyntaxModes/CssSyntaxMode.xml \
	SyntaxModes/CSyntaxMode.xml \
	SyntaxModes/DiffSyntaxMode.xml \
	SyntaxModes/ILSyntaxMode.xml \
	SyntaxModes/JavascriptSyntaxMode.xml \
	SyntaxModes/JavaSyntaxMode.xml \
	SyntaxModes/JaySyntaxMode.xml \
	SyntaxModes/JsonSyntaxMode.xml \
	SyntaxModes/LuaSyntaxMode.xml \
	SyntaxModes/MakefileSyntaxMode.xml \
	SyntaxModes/PythonSyntaxMode.xml \
	SyntaxModes/RubySyntaxMode.xml \
	SyntaxModes/ShellScriptSyntaxMode.xml \
	SyntaxModes/StringsSyntaxMode.xml \
	SyntaxModes/ValaSyntaxMode.xml \
	SyntaxModes/VBNetSyntaxMode.xml \
	SyntaxModes/XmlSyntaxMode.xml

all: $(ASSEMBLY) $(ASSEMBLY).mdb $(ASSEMBLY).config

$(ADDIN_BUILD)/%: $(srcdir)/lib/%
	mkdir -p $(ADDIN_BUILD)
	cp $< $@

$(ASSEMBLY): $(build_sources) $(build_resources)
	mkdir -p $(ADDIN_BUILD)
	$(CSC) $(CSC_FLAGS) -unsafe $(REFS) $(build_resources:%=/resource:%) $(build_sources) -out:$@ -target:library

$(ASSEMBLY).mdb: $(ASSEMBLY)

$(ASSEMBLY).config: $(srcdir)/$(CONFIG)
	cp "$(srcdir)/$(CONFIG)" $(ASSEMBLY).config

assemblydir = $(MD_ASSEMBLY_DIR)
assembly_DATA = $(ASSEMBLY) $(ASSEMBLY).mdb $(ASSEMBLY).config

CLEANFILES = $(ASSEMBLY) $(ASSEMBLY).mdb
EXTRA_DIST = $(FILES) $(RES) $(CONFIG)

include $(top_srcdir)/Makefile.include
