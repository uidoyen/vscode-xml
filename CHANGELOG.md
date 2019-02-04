# Change Log

## [0.3.0](https://github.com/redhat-developer/vscode-xml/milestone/3?closed=1) (January 28, 2019)

### Enhancements

* Added ability to format DTD/DOCTYPE content. See [lsp4xml#268](https://github.com/angelozerr/lsp4xml/issues/268).
* Added outline for DTD elements. See [lsp4xml#226](https://github.com/angelozerr/lsp4xml/issues/226).
* XML completion based on internal DTD. See [lsp4xml#251](https://github.com/angelozerr/lsp4xml/issues/251).
* Add `xml.validation.noGrammar` preference, to indicate document won't be validated. See [#89](https://github.com/redhat-developer/vscode-xml/issues/89).
* Provide automatic completion/validation in catalog files. See [#204](https://github.com/redhat-developer/vscode-xml/issues/204).
* Hover for XSI attributes. See [lsp4xml#164](https://github.com/angelozerr/lsp4xml/issues/164).
* Show attribute value completion based on XML Schema/DTD. See [lsp4xml#242](https://github.com/angelozerr/lsp4xml/issues/242).
* Added `xml.format.spaceBeforeEmptyCloseTag` preference to insert whitespace before closing empty end-tag. See [#84](https://github.com/redhat-developer/vscode-xml/issues/84).
* Completion for XSI attributes. See [lsp4xml#163](https://github.com/angelozerr/lsp4xml/issues/163).
* Changing the content of catalog.xml refreshes the catalogs and triggers validation. See [lsp4xml#212](https://github.com/angelozerr/lsp4xml/issues/212).
* Added preference to enable/disable validation `xml.validation.enabled` and `xml.validation.schema`. See [#100](https://github.com/redhat-developer/vscode-xml/pull/100).
* XML completion based on external DTD. See [lsp4xml#106](https://github.com/angelozerr/lsp4xml/issues/106).
* Completion for DTD <!ELEMENT, <!ATTRIBUTE, ... . See [lsp4xml#232](https://github.com/angelozerr/lsp4xml/issues/232).

### Bug Fixes

* Formatting unclosed tag would be in wrong location. See [lsp4xml#269](https://github.com/angelozerr/lsp4xml/issues/269).
* Infinite loop when `<` was typed into an empty DTD file. See [lsp4xml#266](https://github.com/angelozerr/lsp4xml/issues/266).
* Formatting malformed xml removed content. See [#227](https://github.com/redhat-developer/vscode-xml/issues/227).
* Misplace diagnostic for cvc-elt.3.1. See [#241](https://github.com/redhat-developer/vscode-xml/issues/241).
* Adjust range for DTD validation errors. See [#88](https://github.com/redhat-developer/vscode-xml/issues/88).
* XML Schema completion prefix did not work in some cases. See [lsp4xml#214](https://github.com/angelozerr/lsp4xml/issues/214).
* Problems with npm run build-server on Windows. See [#86](https://github.com/redhat-developer/vscode-xml/issues/86).
* XML catalog support apparently not working. See [#78](https://github.com/redhat-developer/vscode-xml/issues/78).
* Formatting removes DOCTYPE's public declaration. See [lsp4xml#250](https://github.com/angelozerr/lsp4xml/issues/250).
* Adjust range error for internal DTD declaration. See [lsp4xml#225](https://github.com/angelozerr/lsp4xml/issues/225).
* Don't add sibling element when completion items is filled with grammar. See [lsp4xml#211](https://github.com/angelozerr/lsp4xml/issues/211).
* Validation needs additional `<uri>` catalog entry. See [lsp4xml#217](https://github.com/angelozerr/lsp4xml/issues/217).
* Support rootUri for XML catalog configuration. See [lsp4xml#206](https://github.com/angelozerr/lsp4xml/issues/206).
* CacheResourcesManager keeps trying to download unavailable resources. See [lsp4xml#201](https://github.com/angelozerr/lsp4xml/issues/201).



## 0.2.0 (November 8, 2018)

### Enhancements

* Prolog completion on first line, by typing: ```<?xml...``` . See [#85](https://github.com/angelozerr/lsp4xml/issues/85).
* Documentation on hover for schema defined attributes. See [#146](https://github.com/angelozerr/lsp4xml/issues/146).
* Faster schema loading. See [#159](https://github.com/angelozerr/lsp4xml/issues/159).
* Autocompletion for XSD's. See [#111](https://github.com/angelozerr/lsp4xml/issues/111).
* Expose server VM arguments in preferences (can configure proxy). See [#169](https://github.com/angelozerr/lsp4xml/issues/169).
* Auto closing tags preference handled with conflicting preference. See [#62](https://github.com/redhat-developer/vscode-xml/pull/62).
* Auto indentation when hitting enter inside an element. See [#52](https://github.com/redhat-developer/vscode-xml/issues/52).
* Document Link support added. See [#56](https://github.com/angelozerr/lsp4xml/issues/56).
* Support for XSL. See [#189](https://github.com/angelozerr/lsp4xml/issues/189).
* Support for completion requests from empty character. See [#112](https://github.com/angelozerr/lsp4xml/issues/112).

### Bug Fixes

* Formatting splitAttributes indentation fix. See [#59](https://github.com/redhat-developer/vscode-xml/issues/59).
* XML content fully preserved on format xml.format.joinContentLines. See [#152](https://github.com/angelozerr/lsp4xml/issues/152).
* Node completion was not working in nested elements. See [#66](https://github.com/redhat-developer/vscode-xml/issues/66).
* End tag completion on empty character. See [#23](https://github.com/redhat-developer/vscode-xml/issues/23).
* Formatting was removing DTD content. See [#198](https://github.com/angelozerr/lsp4xml/issues/198).
* Code action to insert attribute snippet was incorrect. See [#185](https://github.com/angelozerr/lsp4xml/issues/185).
* Completion for XSD was cached too aggressively. See [#194](https://github.com/angelozerr/lsp4xml/issues/194).
* Hover doesnt work when xs:annotation is declared in type. See [#182](https://github.com/angelozerr/lsp4xml/issues/182).
* Incomplete autocompletion for xsl documents. See [#165](https://github.com/angelozerr/lsp4xml/issues/165).
* Validation of non-empty nodes required to be empty shows misplaced diagnostics. See [#147](https://github.com/angelozerr/lsp4xml/issues/147).
* Validation of empty required node shows misplaced diagnostics. See [#145](https://github.com/angelozerr/lsp4xml/issues/145).
* File association should support relative path for systemId. See [#142](https://github.com/angelozerr/lsp4xml/issues/142).
* Code completion is sometimes "one off". See [#80](https://github.com/redhat-developer/vscode-xml/issues/80).
* DTD validation problems not refreshing correctly. See [#79](https://github.com/redhat-developer/vscode-xml/issues/79).
* No validation when referencing a schema in the same directory. See [#144](https://github.com/angelozerr/lsp4xml/issues/144)