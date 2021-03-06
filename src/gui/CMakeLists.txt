
SET(QGIS_GUI_SRCS

raster/qgsrasterminmaxwidget.cpp
raster/qgsrasterrendererwidget.cpp
raster/qgsmultibandcolorrendererwidget.cpp
raster/qgspalettedrendererwidget.cpp
raster/qgssinglebandgrayrendererwidget.cpp
raster/qgssinglebandpseudocolorrendererwidget.cpp
raster/qgsrasterhistogramwidget.cpp

symbology-ng/qgsbrushstylecombobox.cpp
symbology-ng/qgscolorrampcombobox.cpp
symbology-ng/qgsdashspacedialog.cpp
symbology-ng/qgsdatadefinedsymboldialog.cpp
symbology-ng/qgspenstylecombobox.cpp
symbology-ng/qgssymbollayerv2widget.cpp
symbology-ng/qgsrendererv2widget.cpp
symbology-ng/qgssinglesymbolrendererv2widget.cpp
symbology-ng/qgscategorizedsymbolrendererv2widget.cpp
symbology-ng/qgsgraduatedsymbolrendererv2widget.cpp
symbology-ng/qgsrulebasedrendererv2widget.cpp
symbology-ng/qgsrendererv2propertiesdialog.cpp
symbology-ng/qgsstylev2managerdialog.cpp
symbology-ng/qgssymbollevelsv2dialog.cpp
symbology-ng/qgssymbolv2selectordialog.cpp
symbology-ng/qgsvectorgradientcolorrampv2dialog.cpp
symbology-ng/qgsvectorrandomcolorrampv2dialog.cpp
symbology-ng/qgsvectorcolorbrewercolorrampv2dialog.cpp
symbology-ng/qgscptcitycolorrampv2dialog.cpp
symbology-ng/characterwidget.cpp
symbology-ng/qgsstylev2exportimportdialog.cpp
symbology-ng/qgsellipsesymbollayerv2widget.cpp
symbology-ng/qgspointdisplacementrendererwidget.cpp
symbology-ng/qgsvectorfieldsymbollayerwidget.cpp
symbology-ng/qgssymbolslistwidget.cpp
symbology-ng/qgssvgselectorwidget.cpp
symbology-ng/qgslayerpropertieswidget.cpp
symbology-ng/qgssmartgroupeditordialog.cpp

attributetable/qgsattributetabledelegate.cpp
attributetable/qgsattributetablefiltermodel.cpp
attributetable/qgsattributetablemodel.cpp
attributetable/qgsattributetableview.cpp
attributetable/qgsdualview.cpp
attributetable/qgsfeaturelistmodel.cpp
attributetable/qgsfeaturelistview.cpp
attributetable/qgsfeaturelistviewdelegate.cpp
attributetable/qgsfeatureselectionmodel.cpp
attributetable/qgsgenericfeatureselectionmanager.cpp
attributetable/qgsvectorlayerselectionmanager.cpp

editorwidgets/core/qgseditorconfigwidget.cpp
editorwidgets/core/qgseditorwidgetfactory.cpp
editorwidgets/core/qgseditorwidgetregistry.cpp
editorwidgets/core/qgseditorwidgetwrapper.cpp
editorwidgets/qgsrelationreferencewidget.cpp
editorwidgets/qgsrelationreferencefactory.cpp
editorwidgets/qgsrelreferenceconfigdlg.cpp

qgisgui.cpp
qgisinterface.cpp
qgsannotationitem.cpp
qgsattributedialog.cpp
qgsattributeeditor.cpp
qgsattributeeditorcontext.cpp
qgsblendmodecombobox.cpp
qgsbusyindicatordialog.cpp
qgscharacterselectdialog.cpp
qgscollapsiblegroupbox.cpp
qgscolorbutton.cpp
qgscolordialog.cpp
qgscomposerruler.cpp
qgscomposerview.cpp
qgscredentialdialog.cpp
qgscursors.cpp
qgsdatadefinedbutton.cpp
qgsdetaileditemdata.cpp
qgsdatumtransformdialog.cpp
qgsdetaileditemdelegate.cpp
qgsdetaileditemwidget.cpp
qgsdialog.cpp
qgsencodingfiledialog.cpp
qgserrordialog.cpp
qgsexpressionbuilderdialog.cpp
qgsexpressionbuilderwidget.cpp
qgsexpressionhighlighter.cpp
qgsexpressionselectiondialog.cpp
qgsextentgroupbox.cpp
qgsfeatureselectiondlg.cpp
qgsfieldcombobox.cpp
qgsfieldexpressionwidget.cpp
qgsfieldmodel.cpp
qgsfieldvalidator.cpp
qgsfiledropedit.cpp
qgsfilterlineedit.cpp
qgsformannotationitem.cpp
qgsgenericprojectionselector.cpp
qgshighlight.cpp
qgshtmlannotationitem.cpp
qgslegendinterface.cpp
qgsludialog.cpp
qgsmanageconnectionsdialog.cpp
qgsmapcanvas.cpp
qgsmapcanvasitem.cpp
qgsmapcanvasmap.cpp
qgsmapcanvassnapper.cpp
qgsmaplayeractionregistry.cpp
qgsmaplayercombobox.cpp
qgsmaplayermodel.cpp
qgsmaplayerproxymodel.cpp
qgsmapoverviewcanvas.cpp
qgsmaptip.cpp
qgsmaptool.cpp
qgsmaptoolemitpoint.cpp
qgsmaptoolidentify.cpp
qgsmaptoolpan.cpp
qgsmaptoolzoom.cpp
qgsmessagebar.cpp
qgsmessagebaritem.cpp
qgsmessagelogviewer.cpp
qgsmessageviewer.cpp
qgsnewhttpconnection.cpp
qgsnewvectorlayerdialog.cpp
qgsnumericsortlistviewitem.cpp
qgsoptionsdialogbase.cpp
qgsowssourceselect.cpp
qgspluginmanagerinterface.cpp
qgsprojectbadlayerguihandler.cpp
qgsprojectionselector.cpp
qgsquerybuilder.cpp
qgsrasterformatsaveoptionswidget.cpp
qgsrasterlayersaveasdialog.cpp
qgsrasterpyramidsoptionswidget.cpp
qgsrelationadddlg.cpp
qgsrelationeditor.cpp
qgsrelationmanagerdialog.cpp
qgsrubberband.cpp
qgsscalecombobox.cpp
qgssearchquerybuilder.cpp
qgssublayersdialog.cpp
qgssvgannotationitem.cpp
qgstextannotationitem.cpp
qgsvertexmarker.cpp
qgsunitselectionwidget.cpp
)

IF (WITH_TOUCH)
  SET(QGIS_GUI_SRCS
      ${QGIS_GUI_SRCS}
      qgsmaptooltouch.cpp
  )
ENDIF (WITH_TOUCH)

SET(QGIS_GUI_MOC_HDRS

qgscolorbutton.h

raster/qgsrasterminmaxwidget.h
raster/qgspalettedrendererwidget.h
raster/qgsmultibandcolorrendererwidget.h
raster/qgssinglebandgrayrendererwidget.h
raster/qgssinglebandpseudocolorrendererwidget.h
raster/qgsrasterhistogramwidget.h

symbology-ng/qgsdashspacedialog.h
symbology-ng/qgssymbollayerv2widget.h
symbology-ng/qgssinglesymbolrendererv2widget.h
symbology-ng/qgscategorizedsymbolrendererv2widget.h
symbology-ng/qgsdatadefinedsymboldialog.h
symbology-ng/qgsgraduatedsymbolrendererv2widget.h
symbology-ng/qgsrulebasedrendererv2widget.h
symbology-ng/qgsrendererv2widget.h
symbology-ng/qgsrendererv2propertiesdialog.h
symbology-ng/qgsstylev2managerdialog.h
symbology-ng/qgssymbollevelsv2dialog.h
symbology-ng/qgssymbolv2selectordialog.h
symbology-ng/qgsvectorgradientcolorrampv2dialog.h
symbology-ng/qgsvectorrandomcolorrampv2dialog.h
symbology-ng/qgsvectorcolorbrewercolorrampv2dialog.h
symbology-ng/qgscptcitycolorrampv2dialog.h
symbology-ng/qgscolorrampcombobox.h
symbology-ng/characterwidget.h
symbology-ng/qgspenstylecombobox.h
symbology-ng/qgsbrushstylecombobox.h
symbology-ng/qgsstylev2exportimportdialog.h
symbology-ng/qgsellipsesymbollayerv2widget.h
symbology-ng/qgspointdisplacementrendererwidget.h
symbology-ng/qgsvectorfieldsymbollayerwidget.h
symbology-ng/qgssymbolslistwidget.h
symbology-ng/qgssvgselectorwidget.h
symbology-ng/qgslayerpropertieswidget.h
symbology-ng/qgssmartgroupeditordialog.h

attributetable/qgsattributetabledelegate.h
attributetable/qgsattributetablefiltermodel.h
attributetable/qgsattributetablemodel.h
attributetable/qgsattributetableview.h
attributetable/qgsdualview.h
attributetable/qgsfeaturelistmodel.h
attributetable/qgsfeaturelistview.h
attributetable/qgsfeaturelistviewdelegate.h
attributetable/qgsfeatureselectionmodel.h
attributetable/qgsgenericfeatureselectionmanager.h
attributetable/qgsifeatureselectionmanager.h
attributetable/qgsvectorlayerselectionmanager.h

editorwidgets/core/qgseditorconfigwidget.h
editorwidgets/core/qgseditorwidgetregistry.h
editorwidgets/core/qgseditorwidgetwrapper.h
editorwidgets/qgsrelationreferencewidget.h
editorwidgets/qgsrelreferenceconfigdlg.h

qgisinterface.h
qgsattributedialog.h
qgsattributeeditor.h
qgsblendmodecombobox.h
qgsbusyindicatordialog.h
qgscharacterselectdialog.h
qgscollapsiblegroupbox.h
qgscolordialog.h
qgscomposerruler.h
qgscomposerview.h
qgscredentialdialog.h
qgsdatadefinedbutton.h
qgsdatumtransformdialog.h
qgsdetaileditemdelegate.h
qgsdetaileditemwidget.h
qgsdialog.h
qgsencodingfiledialog.h
qgserrordialog.h
qgsexpressionbuilderwidget.h
qgsexpressionhighlighter.h
qgsexpressionselectiondialog.h
qgsextentgroupbox.h
qgsfeatureselectiondlg.h
qgsfieldcombobox.h
qgsfieldexpressionwidget.h
qgsfieldmodel.h
qgsfieldvalidator.h
qgsfilterlineedit.h
qgsformannotationitem.h
qgsgenericprojectionselector.h
qgshtmlannotationitem.h
qgslegendinterface.h
qgslonglongvalidator.h
qgsludialog.h
qgsmanageconnectionsdialog.h
qgsmapcanvas.h
qgsmaplayeractionregistry.h
qgsmaplayercombobox.h
qgsmaplayermodel.h
qgsmaplayerproxymodel.h
qgsmapoverviewcanvas.h
qgsmaptool.h
qgsmaptoolemitpoint.h
qgsmaptoolidentify.h
qgsmessagebaritem.h
qgsmessagebar.h
qgsmessagelogviewer.h
qgsmessageviewer.h
qgsnewhttpconnection.h
qgsnewvectorlayerdialog.h
qgsoptionsdialogbase.h
qgsowssourceselect.h
qgspluginmanagerinterface.h
qgsprojectbadlayerguihandler.h
qgsprojectionselector.h
qgsquerybuilder.h
qgsrasterformatsaveoptionswidget.h
qgsrasterlayersaveasdialog.h
qgsrasterpyramidsoptionswidget.h
qgsrelationadddlg.h
qgsrelationeditor.h
qgsrelationmanagerdialog.h
qgsscalecombobox.h
qgssearchquerybuilder.h
qgssublayersdialog.h
qgsunitselectionwidget.h
)

QT4_WRAP_CPP(QGIS_GUI_MOC_SRCS ${QGIS_GUI_MOC_HDRS})

IF(UNIX)
  SET_SOURCE_FILES_PROPERTIES(${QGIS_GUI_MOC_SRCS} PROPERTIES COMPILE_FLAGS "-Wno-deprecated-declarations" )
ENDIF(UNIX)

# for installing headers

SET(QGIS_GUI_HDRS
qgisgui.h
qgisinterface.h
qgsattributeeditor.h
qgsattributedialog.h
qgsattributeeditorcontext.h
qgsbusyindicatordialog.h
qgscharacterselectdialog.h
qgscollapsiblegroupbox.h
qgscolordialog.h
qgscredentialdialog.h
qgscursors.h
qgsdatadefinedbutton.h
qgsencodingfiledialog.h
qgsexpressionbuilderdialog.h
qgsexpressionbuilderwidget.h
qgsexpressionhighlighter.h
qgsexpressionselectiondialog.h
qgsfeatureselectiondlg.h
qgsfieldcombobox.h
qgsfieldexpressionwidget.h
qgsfieldmodel.h
qgsfieldvalidator.h
qgsfiledropedit.h
qgsfilterlineedit.h
qgsgenericprojectionselector.h
qgshighlight.h
qgsmapcanvas.h
qgsmapcanvasitem.h
qgsmapcanvasmap.h
qgsmapcanvassnapper.h
qgsmaplayercombobox.h
qgsmaplayermodel.h
qgsmaplayerproxymodel.h
qgsmapoverviewcanvas.h
qgsmaptip.h
qgsmaptool.h
qgsmaptoolemitpoint.h
qgsmaptoolidentify.h
qgsmaptoolpan.h
qgsmaptoolzoom.h
qgsmessagebaritem.h
qgsmessagebar.h
qgsmessageviewer.h
qgsoptionsdialogbase.h
qgsowssourceselect.h
qgsprojectionselector.h
qgsrelationeditor.h
qgsrubberband.h
qgsscalecombobox.h
qgssearchquerybuilder.h
qgssublayersdialog.h
qgsvectorlayertools.h
qgsvertexmarker.h
qgsnumericsortlistviewitem.h
qgsannotationitem.h
qgstextannotationitem.h
qgssvgannotationitem.h
qgscomposerruler.h
qgsdetaileditemdata.h
qgsunitselectionwidget.h

attributetable/qgsattributetabledelegate.h
attributetable/qgsattributetablefiltermodel.h
attributetable/qgsattributetablemodel.h
attributetable/qgsattributetableview.h
attributetable/qgsdualview.h
attributetable/qgsfeaturelistmodel.h
attributetable/qgsfeaturelistview.h
attributetable/qgsfeaturelistviewdelegate.h
attributetable/qgsfeaturemodel.h
attributetable/qgsfeatureselectionmodel.h
attributetable/qgsgenericfeatureselectionmanager.h
attributetable/qgsifeatureselectionmanager.h
attributetable/qgsvectorlayerselectionmanager.h

editorwidgets/core/qgseditorconfigwidget.h
editorwidgets/core/qgseditorwidgetfactory.h
editorwidgets/core/qgseditorwidgetregistry.h
editorwidgets/core/qgseditorwidgetwrapper.h
editorwidgets/qgsrelationreferencefactory.h
editorwidgets/qgsrelationreferencewidget.h
editorwidgets/qgsrelreferenceconfigdlg.h

raster/qgsrasterrendererwidget.h
)

IF (WITH_TOUCH)
  SET(QGIS_GUI_HDRS
      ${QGIS_GUI_HDRS}
      qgsmaptooltouch.h
  )
ENDIF (WITH_TOUCH)

SET(QGIS_GUI_UI_HDRS
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsdetaileditemwidgetbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsgenericprojectionselectorbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsmessageviewer.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsmessagelogviewer.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsowssourceselectbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgscredentialdialog.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsprojectionselectorbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsquerybuilderbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsexpressionbuilder.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsexpressionbuilderdialogbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgsexpressionselectiondialogbase.h
${CMAKE_CURRENT_BINARY_DIR}/../ui/ui_qgssublayersdialogbase.h
)

# ModelTest
#SET(MODELTEST_SRCS
#  ../../tests/qt_modeltest/modeltest.cpp
#  ../../tests/qt_modeltest/dynamictreemodel.cpp
#)
#SET(MODELTEST_MOC_HDRS
#  ../../tests/qt_modeltest/modeltest.h
#  ../../tests/qt_modeltest/dynamictreemodel.h
#)
#QT4_WRAP_CPP(MODELTEST_MOC_SRCS ${MODELTEST_MOC_HDRS})
#INCLUDE_DIRECTORIES(../../tests/qt_modeltest)


INCLUDE_DIRECTORIES(
  ${QT_QTUITOOLS_INCLUDE_DIR}
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${CMAKE_CURRENT_SOURCE_DIR}/symbology-ng
  ${CMAKE_CURRENT_SOURCE_DIR}/attributetable
  ${CMAKE_CURRENT_SOURCE_DIR}/editorwidgets
  ${CMAKE_CURRENT_SOURCE_DIR}/editorwidgets/core
  ../core
  ../core/composer
  ../core/raster
  ../core/symbology-ng
  ${CMAKE_CURRENT_BINARY_DIR}
  ${CMAKE_CURRENT_BINARY_DIR}/../ui
  ${QWT_INCLUDE_DIR}
)
IF (WITH_INTERNAL_SPATIALITE)
  INCLUDE_DIRECTORIES(../core/spatialite/headers)
  INCLUDE_DIRECTORIES(../core/spatialite/headers/spatialite)
ELSE (WITH_INTERNAL_SPATIALITE)
  INCLUDE_DIRECTORIES(${SQLITE3_INCLUDE_DIR})
ENDIF (WITH_INTERNAL_SPATIALITE)

INCLUDE_DIRECTORIES(${GEOS_INCLUDE_DIR})
INCLUDE_DIRECTORIES(${GDAL_INCLUDE_DIR})

IF (WIN32)
  IF (MSVC)
    ADD_DEFINITIONS("-DGUI_EXPORT=${DLLEXPORT}")
  ELSE (MSVC)
    ADD_DEFINITIONS("-UGUI_EXPORT \"-DGUI_EXPORT=${DLLEXPORT}\"")
  ENDIF (MSVC)
ENDIF (WIN32)

# disable deprecation warnings for classes re-exporting deprecated methods
IF(MSVC)
  SET_SOURCE_FILES_PROPERTIES(
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgisinterface.cxx
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgsgenericprojectionselector.cxx
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgsprojectionselector.cxx
    PROPERTIES COMPILE_FLAGS "-wd4996")
ELSE(MSVC)
  SET_SOURCE_FILES_PROPERTIES(
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgisinterface.cxx
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgsgenericprojectionselector.cxx
    ${CMAKE_BINARY_DIR}/src/gui/moc_qgsprojectionselector.cxx
    PROPERTIES COMPILE_FLAGS "-w -Wno-deprecated-declarations")
ENDIF(MSVC)

#############################################################
# qgis_gui library

ADD_LIBRARY(qgis_gui SHARED
     ${QGIS_GUI_SRCS} ${QGIS_GUI_MOC_SRCS} ${QGIS_GUI_HDRS} ${QGIS_GUI_MOC_HDRS}
     #${MODELTEST_SRCS} ${MODELTEST_MOC_SRCS}  # for ModelTest
)

IF(NOT APPLE)
  INSTALL(FILES ${QGIS_GUI_HDRS} ${QGIS_GUI_MOC_HDRS} DESTINATION ${QGIS_INCLUDE_DIR})
ELSE(NOT APPLE)
  SET_TARGET_PROPERTIES(qgis_gui PROPERTIES
    CLEAN_DIRECT_OUTPUT 1
    FRAMEWORK 1
    FRAMEWORK_VERSION "${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}"
    MACOSX_FRAMEWORK_INFO_PLIST "${CMAKE_SOURCE_DIR}/mac/framework.info.plist.in"
    MACOSX_FRAMEWORK_SHORT_VERSION_STRING ${COMPLETE_VERSION}
    MACOSX_FRAMEWORK_IDENTIFIER org.qgis.qgis2_gui
    BUILD_WITH_INSTALL_RPATH TRUE
    PUBLIC_HEADER "${QGIS_GUI_HDRS};${QGIS_GUI_MOC_HDRS}"
    LINK_FLAGS "${CMAKE_SHARED_LINKER_FLAGS}"
  )
ENDIF(NOT APPLE)

#generate unversioned libs for android
IF (NOT ANDROID)
  SET_TARGET_PROPERTIES(qgis_gui PROPERTIES
    VERSION ${COMPLETE_VERSION}
    SOVERSION ${COMPLETE_VERSION}
    )
ENDIF (NOT ANDROID)

# make sure that UI files will be processed first
ADD_DEPENDENCIES(qgis_gui ui)

TARGET_LINK_LIBRARIES(qgis_gui
  qgis_core
  ${QT_QTUITOOLS_LIBRARY}
  ${QWT_LIBRARY}
  #${QT_QTTEST_LIBRARY}  # for ModelTest
)

IF(WIN32)
  ADD_DEFINITIONS(-DQWT_DLL)
ENDIF(WIN32)

# install

INSTALL(TARGETS qgis_gui
  RUNTIME DESTINATION ${QGIS_BIN_DIR}
  LIBRARY DESTINATION ${QGIS_LIB_DIR}
  ARCHIVE DESTINATION ${QGIS_LIB_DIR}
  FRAMEWORK DESTINATION ${QGIS_FW_SUBDIR}
  PUBLIC_HEADER DESTINATION ${QGIS_INCLUDE_DIR})

# ui headers to install, don't exist at target definition time, install manually
IF (APPLE)
  INSTALL(FILES ${QGIS_GUI_UI_HDRS} DESTINATION ${QGIS_FW_SUBDIR}/qgis_gui.framework/Headers)
ELSE (APPLE)
  INSTALL(FILES ${QGIS_GUI_UI_HDRS} DESTINATION ${QGIS_INCLUDE_DIR})
ENDIF (APPLE)

# Mac dev frameworks

IF (APPLE AND QGIS_MACAPP_INSTALL_DEV)
  INSTALL(TARGETS qgis_gui FRAMEWORK DESTINATION ${QGIS_MACAPP_DEV_PREFIX})
  INSTALL(FILES ${QGIS_GUI_UI_HDRS} DESTINATION ${QGIS_MACAPP_DEV_PREFIX}/qgis_gui.framework/Headers)
  INSTALL(CODE "EXECUTE_PROCESS(COMMAND install_name_tool -id \"${QGIS_MACAPP_DEV_PREFIX}/qgis_gui.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_gui\" \"$ENV{DESTDIR}${QGIS_MACAPP_DEV_PREFIX}/qgis_gui.framework/qgis_gui\")")
  INSTALL(CODE "EXECUTE_PROCESS(COMMAND install_name_tool -change \"${CMAKE_INSTALL_NAME_DIR}/qgis_core.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_core\" \"${QGIS_MACAPP_DEV_PREFIX}/qgis_core.framework/Versions/${CPACK_PACKAGE_VERSION_MAJOR}.${CPACK_PACKAGE_VERSION_MINOR}/qgis_core\" \"$ENV{DESTDIR}${QGIS_MACAPP_DEV_PREFIX}/qgis_gui.framework/qgis_gui\")")
ENDIF (APPLE AND QGIS_MACAPP_INSTALL_DEV)
