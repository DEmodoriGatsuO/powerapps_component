# Power Apps YAML Source Code: File Uploader Component

## Overview

This repository contains the YAML source code for the `cmp_file_uploader` component in Power Apps. This component is designed to facilitate file uploads to SharePoint, utilizing a predefined set of file types and extensions for better user experience.

## Component Structure

### Component: `cmp_file_uploader`

- **Control**: Component
- **Properties**:
  - `drive_id`: SharePoint drive ID
  - `folder_name`: Name of the folder
  - `site_id`: SharePoint site ID
  - `static_icon_table`: Table defining file types and their extensions

### Custom Properties

- `site_id`: SharePoint SiteId (Input)
- `drive_id`: SharePoint Drive ID (Input)
- `folder_name`: Folder Name (Input)
- `static_icon_table`: Table defining file types and extensions (Input)
- `response`: Custom property for responses (Output)

### Reference
- [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) - https://developer.microsoft.com/en-us/graph/graph-explorer
- [Power Apps DIRECTLY upload files to SharePoint Document Library | GRAPH API](https://youtu.be/n3mhe88BI34?si=xtlIrg0u84fLQP-Q) - https://youtu.be/n3mhe88BI34?si=xtlIrg0u84fLQP-Q
- [Error、IfError、IsError、IsBlankOrError 関数](https://learn.microsoft.com/ja-jp/power-platform/power-fx/reference/function-iferror) - https://learn.microsoft.com/ja-jp/power-platform/power-fx/reference/function-iferror
- [Office 365 Groups](https://learn.microsoft.com/ja-jp/connectors/office365groups/) - https://learn.microsoft.com/ja-jp/connectors/office365groups/

<iframe width="560" height="315" src="https://www.youtube.com/embed/n3mhe88BI34?si=xtlIrg0u84fLQP-Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Children

1. **Container: `con_component`**
   - **Control**: GroupContainer
   - **Variant**: verticalAutoLayoutContainer
   - **Properties**: Layout and styling properties for the container
   - **Children**:
     1. **Upload Area: `ico_upload_area`**
        - **Control**: GroupContainer
        - **Variant**: verticalAutoLayoutContainer
        - **Properties**: Layout and styling properties for the upload area
        - **Children**:
          - **Upload Header: `con_upload_header`**
            - **Control**: GroupContainer
            - **Variant**: horizontalAutoLayoutContainer
            - **Properties**: Layout and styling properties for the header
            - **Children**:
              - **Icon: `ico_upload_header`**
                - **Control**: Classic/Icon
                - **Variant**: Download
                - **Properties**: Icon properties including selection action
              - **Label: `lbl_upload_header`**
                - **Control**: Label
                - **Properties**: Text and styling properties
          - **Attachment: `attach_files`**
            - **Control**: Attachments
            - **Properties**: Properties related to file attachments and actions
          - **Shape: `shp_upload_area`**
            - **Control**: Rectangle
            - **Properties**: Layout and styling properties
          - **Path: `con_path`**
            - **Control**: GroupContainer
            - **Variant**: horizontalAutoLayoutContainer
            - **Properties**: Layout and styling properties for the path
            - **Children**:
              - **Document Library Label: `lbl_documentlibrary`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **Icon: `ico_chevron`**
                - **Control**: Classic/Icon
                - **Variant**: ChevronRight
                - **Properties**: Icon properties
              - **Folder Label: `lbl_folder`**
                - **Control**: Label
                - **Properties**: Text and styling properties
          - **Gallery Header: `con_gal_header`**
            - **Control**: GroupContainer
            - **Variant**: horizontalAutoLayoutContainer
            - **Properties**: Layout and styling properties for the gallery header
            - **Children**:
              - **File Image: `img_files`**
                - **Control**: Image
                - **Properties**: Image properties
              - **Name Header: `hdr_name`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **Last Modified Date Header: `hdr_lastmodifieddatetime`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **Last Modified By Header: `hdr_lastmodifiedby`**
                - **Control**: Label
                - **Properties**: Text and styling properties
          - **Header Shape: `shp_header`**
            - **Control**: Rectangle
            - **Properties**: Layout and styling properties
          - **Files Gallery: `gal_files`**
            - **Control**: Gallery
            - **Variant**: galleryVertical
            - **Properties**: Gallery properties including items, layout, and actions
            - **Children**:
              - **Last Modified By Label: `lbl_lastmodifiedby`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **Last Modified Date Label: `lbl_lastmodifieddatetime`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **Filename Label: `lbl_filename`**
                - **Control**: Label
                - **Properties**: Text and styling properties
              - **File Type Image: `img_filetype`**
                - **Control**: Image
                - **Properties**: Image properties including selection action
              - **File Gallery Shape: `shp_gal_files`**
                - **Control**: Rectangle
                - **Properties**: Layout and styling properties

## Usage

### Setting Up

1. **Define Properties**: Set the `site_id`, `drive_id`, `folder_name`, and `static_icon_table` properties with appropriate values.
2. **Configure Attachments**: Ensure the `OnAddFile` property in the `Attachments` control is correctly set up to handle file uploads to SharePoint.
3. **Customize Layout**: Adjust the layout and styling properties as needed to fit the design requirements.

### Customization

- **Add New File Types**: Update the `static_icon_table` property to include additional file types and their corresponding extensions.
- **Modify Layout**: Adjust the properties of the GroupContainers, Labels, Icons, and other controls to change the appearance and behavior of the component.
