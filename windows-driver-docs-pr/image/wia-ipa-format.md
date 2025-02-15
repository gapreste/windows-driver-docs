---
title: WIA_IPA_FORMAT
description: The WIA_IPA_FORMAT property contains the current format of the image that is about to be transferred. The WIA minidriver creates and maintains this property.
keywords: ["WIA_IPA_FORMAT Imaging Devices"]
topic_type:
- apiref
api_name:
- WIA_IPA_FORMAT
api_location:
- Wiadef.h
api_type:
- HeaderDef
ms.date: 10/04/2021
ms.localizationpriority: medium
---

# WIA_IPA_FORMAT

The WIA_IPA_FORMAT property contains the current format of the image that is about to be transferred. The WIA minidriver creates and maintains this property.

Property Type: VT_CLSID

Valid Values: WIA_PROP_LIST

Access Rights: Read/write

## Remarks

If you can set the device to only a single value, create a WIA_PROP_LIST type, and place the valid value in it.

For Windows 8 and later versions of Windows, the following values have been added for the WIA_IPA_FORMAT property:

- WiaImgFmt_CSV

- WiaImgFmt_JBIG2

- WiaImgFmt_RawBar

- WiaImgFmt_RawMic

- WiaImgFmt_RawPat

- WiaImgFmt_XmlBar

- WiaImgFmt_XmlMic

- WiaImgFmt_XmlPat

Beginning with Windows Vista and later versions of Windows, the following values are added for the WIA_IPA_FORMAT property:

- WiaImgFmt_PDFA

- WiaImgFmt_JBIG

- WiaImgFmt_XPS

For both the WiaImgFmt_PDFA and WiaImgFmt_XPS formats, the drivers should support any [**WIA_IPA_COMPRESSION**](wia-ipa-compression.md) value. For these two formats, the default WIA_IPA_COMPRESSION value, WIA_COMPRESSION_NONE, means "not defined." The scanner (or the driver, where the PDF/A or XPS file is generated) must choose the internal compression mode that is used for image data.

The following table describes the constants that are valid with WIA_IPA_FORMAT.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Format</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>WiaAudFmt_AIFF</p></td>
<td><p>AIFF audio format</p></td>
</tr>
<tr class="even">
<td><p>WiaAudFmt_MP3</p></td>
<td><p>MP3 audio format</p></td>
</tr>
<tr class="odd">
<td><p>WiaAudFmt_WAV</p></td>
<td><p>WAV audio format</p></td>
</tr>
<tr class="even">
<td><p>WiaAudFmt_WMA</p></td>
<td><p>WMA audio format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_ASF</p></td>
<td><p>ASF video format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_AVI</p></td>
<td><p>AVI video format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_BMP</p></td>
<td><p>Windows Device Independent Bitmap (DIB) file</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_CIFF</p></td>
<td><p>Camera Image File format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_CSV<strong></p></td>
<td><p>Comma separated file</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_DPOF</p></td>
<td><p>DPOF printing format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_EMF</p></td>
<td><p>Extended Windows metafile</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_EXEC</p></td>
<td><p>Executable file</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_EXIF</p></td>
<td><p>Exchangeable File Format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_FLASHPIX</p></td>
<td><p>FlashPix format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_GIF</p></td>
<td><p>GIF image format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_HTML</p></td>
<td><p>HTML format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_ICO</p></td>
<td><p>Windows icon file format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_JBIG*</p></td>
<td><p>Joint Bi-level Image experts Group format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_JBIG2</strong></p></td>
<td><p>Joint Bi-level Image experts Group format (version 2)</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_JPEG</p></td>
<td><p>JPEG compressed format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_JPEG2K</p></td>
<td><p>JPEG 2000 compressed format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_JPEG2KX</p></td>
<td><p>JPEG 2000 compressed format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_MEMORYBMP</p></td>
<td><p>Windows bitmap without a header file</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_MPG</p></td>
<td><p>MPEG video format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_PHOTOCD</p></td>
<td><p>Eastman Kodak file format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_PDFA<em></p></td>
<td><p>PDF/A (ISO/CD 19005-1) format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_PICT</p></td>
<td><p>Apple file format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_PNG</p></td>
<td><p>W3C PNG format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_RAW</p></td>
<td><p>WIA Raw image file format for data transfers only</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_RawBar</em><em></p></td>
<td><p>WIA Barcode Metadata Raw Format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_RawMic</em><em></p></td>
<td><p>WIA MICR Metadata Raw Format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_RawPat</em><em></p></td>
<td><p>WIA Patch Code Metadata Raw Format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_RAWRGB</p></td>
<td><p>Raw RGB format</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_RTF</p></td>
<td><p>Rich Text File format</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_SCRIPT</p></td>
<td><p>Script file</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_TIFF</p></td>
<td><p>Tagged Image File Format (TIFF)</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_TXT</p></td>
<td><p>Text file</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_UNICODE16</p></td>
<td><p>Unicode 16-bit encoding</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_WMF</p></td>
<td><p>Windows metafile</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_XML</p></td>
<td><p>XML file</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_XmlBar</em><em></p></td>
<td><p>XML file whose content is compliant with the WIA Barcode Metadata Schema</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_XmlMic</em><em></p></td>
<td><p>XML file whose content is compliant with the WIA MICR Metadata Schema</p></td>
</tr>
<tr class="odd">
<td><p>WiaImgFmt_XmlPat</em><em></p></td>
<td><p>XML file whose content is compliant with the WIA Patch Code Metadata Schema</p></td>
</tr>
<tr class="even">
<td><p>WiaImgFmt_XPS</em></p></td>
<td><p>XPS document file</p></td>
</tr>
</tbody>
</table>

Formats that are marked with an asterisk (\*) are for Windows Vista and later versions of Windows only.

Formats that are marked with two asterisks (\*\*) are for Windows 8 and later versions of Windows only.

All WIA 2.0 minidrivers must set the initial value of this property to its default value, which is WiaImgFmt_BMP.

## Requirements

**Header:** wiadef.h (include Wiadef.h)

## See also

[**WIA_IPA_COMPRESSION**](wia-ipa-compression.md)

[**WIA_IPA_FULL_ITEM_NAME**](wia-ipa-full-item-name.md)
