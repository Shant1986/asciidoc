# AsciiDoc Quick Reference

## Introduction

Welcome to the AsciiDoc Quick Reference, a guide for mastering AsciiDoc markup.

## Table of Contents

1. [Installation](#installation)
2. [Basic Syntax](#basic-syntax)
   - [Headings](#headings)
   - [Text Formatting](#text-formatting)
   - [Lists](#lists)
   - [Links](#links)
   - [Images](#images)
3. [Advanced Features](#advanced-features)
   - [Tables](#tables)
   - [Code Blocks](#code-blocks)
   - [Admonitions](#admonitions)
   - [Footnotes](#footnotes)
4. [Document Structure](#document-structure)
   - [Front Matter](#front-matter)
   - [Sections](#sections)
   - [Includes](#includes)
5. [Customization](#customization)
   - [Styles](#styles)
   - [Attributes](#attributes)
   - [Document Header](#document-header)
6. [Integration with Other Tools](#integration-with-other-tools)
   - [GitHub Flavored AsciiDoc](#github-flavored-asciidoc)
   - [DocBook Conversion](#docbook-conversion)
7. [Best Practices](#best-practices)
   - [Consistent Naming](#consistent-naming)
   - [Version Control](#version-control)
   - [Collaborative Writing](#collaborative-writing)
8. [Resources](#resources)
   - [Official Documentation](#official-documentation)
   - [Community Forums](#community-forums)
   - [Additional Tutorials](#additional-tutorials)

## 1. Installation <a name="installation"></a>

AsciiDoc doesn't require specific installation. Use any text editor. For enhanced features, consider tools like AsciiDoctor.

```bash
# Install AsciiDoctor on Linux
sudo gem install asciidoctor

## 1. Installation <a name="installation"></a>

AsciiDoc doesn't require specific installation. You can create AsciiDoc files using any text editor. However, for a more feature-rich experience, consider the following options:

### 1.1 Basic Text Editor <a name="basic-text-editor"></a>

You can create AsciiDoc files using any basic text editor, making it a simple and accessible choice for all users. Follow these general steps:

1. Open your preferred text editor. This could be Notepad on Windows, TextEdit on Mac, or Gedit on Linux.
2. Start writing your AsciiDoc content in the editor.
3. Save your files with the `.adoc` extension to indicate they are written in AsciiDoc.

Using a basic text editor is an ideal starting point for getting acquainted with AsciiDoc without the need for additional tools or installations. It is a straightforward approach suitable for quick edits and simple document creation.

### 1.2 Dedicated Editors <a name="dedicated-editors"></a>

For a more feature-rich and efficient AsciiDoc editing experience, you can use dedicated AsciiDoc editors. One popular choice is Visual Studio Code (VS Code) with the AsciiDoc extension. Follow these steps to set up your environment:

1. Install [Visual Studio Code](https://code.visualstudio.com/).
2. Open VS Code and navigate to Extensions (`Ctrl + Shift + X`).
3. Search for "AsciiDoc" and install the extension provided by AsciiDoc.

By using dedicated editors, you gain access to features like syntax highlighting, live preview, and other AsciiDoc-specific tools. This enhances your workflow and makes the creation of AsciiDoc documents more efficient and enjoyable.

### 1.3 Command-Line Tools <a name="command-line-tools"></a>

If you prefer working from the command line, you can use the AsciiDoctor tool to process AsciiDoc files and generate various output formats. Follow these steps to install AsciiDoctor on a Linux system:

```bash
sudo gem install asciidoctor

### 1.4 Online Editors <a name="online-editors"></a>

Several online platforms offer AsciiDoc editing capabilities directly in your web browser. Explore options like [Asciidoctor.js Live Preview](https://asciidoctor.org/playground/asciidoc-js-live-preview/).

Choose an online editor based on your preference for web-based editing. These platforms provide a convenient way to work with AsciiDoc without the need for local installations. Begin creating and previewing your AsciiDoc documents seamlessly.

If you prefer the command line, use the AsciiDoctor tool. Install it on a Linux system with:

```bash
sudo gem install asciidoctor

### 2.2 Text Formatting <a name="text-formatting"></a>

Apply basic text formatting to emphasize and highlight content. AsciiDoc supports *italic*, **bold**, and `monospace` text.

**Example:**

```asciidoc
*Italic Text*
**Bold Text**
`Monospace Text`

### 2.3 Lists <a name="lists"></a>

Create ordered and unordered lists to present information in a structured manner.

**Example:**

```asciidoc
- Unordered Item 1
- Unordered Item 2

1. Ordered Item 1
2. Ordered Item 2

### 2.4 Links <a name="links"></a>

Insert hyperlinks to reference external resources or navigate within the document.

**Example:**

```asciidoc
Link to [AsciiDoc Official Site](http://asciidoc.org)

### 2.5 Images <a name="images"></a>

Embed images to enhance visual content within your document.

**Example:**

```asciidoc
image::image.jpg[Alt Text]

## 3. Advanced Features <a name="advanced-features"></a>

Explore advanced features in AsciiDoc to add richness and functionality to your documents.

### 3.1 Tables <a name="tables"></a>

Tables provide a structured way to present data. Use AsciiDoc's table syntax to create tables with headers, rows, and columns.

**Example:**

```asciidoc
|===
|Header 1 |Header 2 |Header 3

|Row 1, Col 1 |Row 1, Col 2 |Row 1, Col 3
|Row 2, Col 1 |Row 2, Col 2 |Row 2, Col 3
|===

### 3.2 Code Blocks <a name="code-blocks"></a>

Use code blocks to display and highlight code snippets within your document.

**Example:**

```asciidoc
[source,language]
----
// Your code here
function example() {
  return "Hello, AsciiDoc!";
}
----

### 3.3 Admonitions <a name="admonitions"></a>

Admonitions provide a way to emphasize content or provide additional information. Common admonition types include `NOTE`, `TIP`, `WARNING`, and `IMPORTANT`.

**Example:**

```asciidoc
[TIP]
====
This is a helpful tip for your readers.
====

### 3.4 Footnotes <a name="footnotes"></a>

**Example:**

```asciidoc
Here is some text[^1].

[^1]: This is the footnote content.

## 4. Document Structure <a name="document-structure"></a>

Understand the structural elements in AsciiDoc for well-organized documents.

### 4.1 Front Matter <a name="front-matter"></a>

Define metadata and settings at the beginning of your document to provide crucial information.

**Example:**

```asciidoc
= Document Title
:author: Your Name
:date: 2024-01-01

### 4.2 Sections <a name="sections"></a>

**Example:**

```asciidoc
== Section 1
This is the content of Section 1.

== Section 2
Content of Section 2.

### 4.3 Includes <a name="includes"></a>

**Example:**

```asciidoc
include::path/to/external/file.adoc[]

## 5. Customization <a name="customization"></a>

Tailor the appearance and behavior of your AsciiDoc documents with customization options.

### 5.1 Styles <a name="styles"></a>

Apply styles to control the visual presentation of elements in your document.

**Example:**

```asciidoc
[source,asciidoc]
----
This is styled text.
:style: emphasized
----
### 5.2 Attributes <a name="attributes"></a>

**Example:**

```asciidoc
:doctype: book
:icons: font

### 5.3 Document Header <a name="document-header"></a>

**Example:**

```asciidoc
= Document Title
:author: Your Name
:date: 2024-01-01

## 6. Integration with Other Tools <a name="integration-with-other-tools"></a>

Learn how AsciiDoc seamlessly integrates with various tools to enhance your workflow.

### 6.1 GitHub Flavored AsciiDoc <a name="github-flavored-asciidoc"></a>

Leverage GitHub Flavored AsciiDoc for rendering AsciiDoc files directly on GitHub.

**Example:**

```asciidoc
.GitHub Flavored AsciiDoc
====
This content is GitHub Flavored AsciiDoc.
====

### 6.2 DocBook Conversion <a name="docbook-conversion"></a>

**Example:**

```asciidoc
:backend: docbook

## 7. Best Practices <a name="best-practices"></a>

Follow these best practices to enhance the effectiveness and maintainability of your AsciiDoc documents.

### 7.1 Consistent Naming <a name="consistent-naming"></a>

Adopt a consistent naming convention for files, sections, and elements within your documents.

**Example:**

```asciidoc
// Consistent file naming
include::chapter-1.adoc[]

== Section Title
Content of the section.

### 7.2 Version Control <a name="version-control"></a>

**Example:**

```bash
git commit -m "Updated documentation"

### 7.3 Collaborative Writing <a name="collaborative-writing"></a>

**Example:**

```asciidoc
// Collaborative comment
// Author: Collaborator1
// Review: Address formatting issues

## 8. Resources <a name="resources"></a>

Explore additional resources to deepen your understanding and proficiency in AsciiDoc.

### 8.1 Official Documentation <a name="official-documentation"></a>

Refer to the official AsciiDoc documentation for comprehensive guidance and reference.

**Link:**
[AsciiDoc Official Documentation](http://asciidoc.org/documentation.html)

### 8.2 Community Forums <a name="community-forums"></a>

Engage with the AsciiDoc community through forums to seek help and share knowledge.

**Link:**
[AsciiDoc Community Forums](http://asciidoctor.976.n4.nabble.com/AsciiDoc-f976.html)

### 8.3 Additional Tutorials <a name="additional-tutorials"></a>

Explore supplementary tutorials and guides to enhance your AsciiDoc skills.

**Link:**
[Additional AsciiDoc Tutorials](https://github.com/asciidoctor/asciidoctor.org/blob/master/CONTRIBUTING.adoc)

Continuously expanding your knowledge with these resources will empower you to master AsciiDoc and create sophisticated documents.
