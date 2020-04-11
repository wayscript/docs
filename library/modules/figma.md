---
description: >-
  Seamlessly integrate Figma with your favorite APIs, databases, and programming
  languages, using WayScript.
---

# Figma

![A collaborative interface design tool.](../../.gitbook/assets/figma.png)

{% hint style="info" %}
Each section links to the corresponding information in the [Figma API documentation](https://www.figma.com/developers/api). Refer there for additional details.
{% endhint %}

## [Figma Files](https://www.figma.com/developers/api#files)

### [GET File](https://www.figma.com/developers/api#get-files-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

#### Optional Inputs

* **Version** \(Advanced\) - A specific version ID to get. Omitting this will get the current version of the file.
* **IDs** - A comma separated list of nodes that you care about in the document. If specified, only a subset of the document will be returned corresponding to the nodes listed, their children, and everything between the root node and the listed nodes.
* **Depth** \(Advanced\) - Positive integer representing how deep into the document tree to traverse. For example, setting this to 1 returns only Pages, setting it to 2 returns Pages and all top level objects on each page. Not setting this parameter returns all nodes.
* **Geometry** \(Advanced\) - Set to 'paths' to export vector data.
* **Plugin Data** \(Advanced\) - A comma separated list of plugin IDs and/or the string 'shared'. Any data present in the document written by those plugins will be included in the result in the `pluginData` and `sharedPluginData` properties.

### [GET File Nodes](https://www.figma.com/developers/api#get-file-nodes-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)
* **IDs**

### [GET Image](https://www.figma.com/developers/api#get-images-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)
* **IDs**

#### Advanced Inputs

* **Version** - A specific version ID to get. Omitting this will get the current version of the file.
* **Scale** - A number between 0.01 and 4, the image scaling factor.
* **Format** - A string enum for the image output format, can be jpg, png, svg, or pdf.
* **SVG Include Id** - Whether to include id attributes for all SVG elements. Default: false.
* **SVG Simplify Stroke** - Whether to simplify inside/outside strokes and use stroke attribute if possible instead of `<mask>`. Default: true.
* **Use Absolute Bounds** - Use the full dimensions of the node regardless of whether or not it is cropped or the space around it is empty. Use this to export text nodes without cropping. Default: false.

### [GET Image Fills](https://www.figma.com/developers/api#get-image-fills-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

## [Comments](https://www.figma.com/developers/api#comments)

### [GET Comments](https://www.figma.com/developers/api#get-comments-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

### [POST Comments](https://www.figma.com/developers/api#post-comments-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)
* **Message -** The text contents of the comment to post

**Optional Inputs**

* **Comment Key** - The comment to reply to, if any. This must be a root comment, that is, you cannot reply to a comment that is a reply itself \(a reply has a parent\_id\).

**Advanced Inputs**

* **Client Meta** - The position of where to place the comment. This can either be an absolute canvas position or the relative position within a frame.

### [DELETE Comments](https://www.figma.com/developers/api#delete-comments-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)
* **Comment Key** - Comment id of comment to delete.

## [Users](https://www.figma.com/developers/api#users)

### [GET Me](https://www.figma.com/developers/api#get-me-endpoint)

Returns the information corresponding to the authenticated user.

## [Version History](https://www.figma.com/developers/api#version-history)

### [GET File Versions](https://www.figma.com/developers/api#get-file-versions-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

## [Projects](https://www.figma.com/developers/api#projects)

### [GET Team Projects](https://www.figma.com/developers/api#get-team-projects-endpoint)

#### **Required Inputs**

* [**Team ID**](figma.md#team-id)

### [GET Project Files](https://www.figma.com/developers/api#get-project-files-endpoint)

#### **Required Inputs**

* [**Project ID**](figma.md#project-id)

## [Components and Styles](https://www.figma.com/developers/api#library-items)

### [GET Team Components](https://www.figma.com/developers/api#get-team-components-endpoint)

#### **Required Inputs**

* [**Team ID**](figma.md#team-id)

#### Advanced Inputs

* **Page Size** - Number of items in a paged list of results. Defaults to 30.

### [GET File Components](https://www.figma.com/developers/api#get-file-components-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

### [GET Component](https://www.figma.com/developers/api#get-component-endpoint)

#### **Required Inputs**

* **Key** - The unique identifier of the component.

### [GET Team Styles](https://www.figma.com/developers/api#get-team-styles-endpoint)

#### **Required Inputs**

* [**Team ID**](figma.md#team-id)

#### Advanced Inputs

* **Page Size** - Number of items in a paged list of results. Defaults to 30.

### [GET File Styles](https://www.figma.com/developers/api#get-file-styles-endpoint)

#### **Required Inputs**

* [**File Key**](figma.md#file-key)

### [GET Style](https://www.figma.com/developers/api#get-style-endpoint)

#### **Required Inputs**

* **Key** - The unique identifier of the style.

## Finding Input Values

### File Key

To find the key for the file you want to work with, open the file in Figma and obtain the key from the URL in your browser. For example, suppose you are looking for the key for your "UI Pieces" file. You should see a url like this in your browser:

`https://www.figma.com/file/JY61PlSmmoRiEHvyrWa4bn/UI-Pieces`

The file key is the portion of the portion of the URL after `file/`: **JY61PlSmmoRiEHvyrWa4bn**

### **Team ID**

Obtain a team ID by navigating to the team in Figma and extracting the ID from the URL. For example, if you are a member of the "WayScript" team, you can navigate to that team in your browser and you should see a URL like this:

`https://www.figma.com/files/team/757969426722171844/Wayscript`

The team ID is the portion of the URL after `team/`: **757969426722171844**

### **Project ID**

Obtain a project ID by navigating to the project in Figma and extracting the ID from the URL. For example, if you are viewing the "Script Editor" project, you should see a URL like this:

`https://www.figma.com/files/project/4073612/Script-Editor`

The project ID is the portion of the URL after `project/`: **4073612**

