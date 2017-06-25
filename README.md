# FORK

This a fork of https://github.com/dragon66/pixymeta to have a versioned artifact with sources.

[ ![Download](https://api.bintray.com/packages/jmoore/java-lib/pixymeta/images/download.svg) ](https://bintray.com/jmoore/java-lib/pixymeta/_latestVersion)

# pixymeta
Java image metadata CRUD tool - a pure Java image metadata manipulation tool.
This is the meta data related part branched out from icafe repository.

Image metadata manipulation:
----------------------------------------
- JPEG and TIFF EXIF data manipulation
   * Insert EXIF data into JPEG.
   * Extract EXIF data from JPEG.
   * Remove EXIF data and other insignificant APPn segments from JPEG.
   * Insert EXIF data into TIFF.
   * Read EXIF data embedded in TIFF.
- JPEG and TIFF ICC Profile support
   * Insert ICC profile to JPEG and TIFF.
   * Extract ICC profile from JPEG and TIFF.
- JPEG and TIFF IPTC metadata support
   * Insert IPTC directly to TIFF via RichTiffIPTC tag.
   * Insert IPTC to JPEG via APP13 Photoshop IRB
   * Extract IPTC from both TIFF and JPEG
- JPEG and TIFF Photoshop IRB metadata support
   * Insert IRB into JPEG via APP13 segment
   * Insert IRB into TIFF via tag PHOTOSHOP.
   * Extract IRB data from both JPEG and TIFF.
- JPEG, GIF, PNG, TIFF XMP metadata support
   * Insert XMP metada into JPEG, GIF, PNG, and TIFF image
   * Extract XMP metadata from JPEG, GIF, PNG, and TIFF image
   * In case of JPEG, handle normal XMP and extendedXMP which cannot fit into one APP1 segment


Where can I get the latest release?
-----------------------------------
Add to your pom.xml:

```xml
<repositories>
    <repository>
      <id>jai-imageio</id>
      <name>Java Advanced Imaging for ImageIO</name>
      <url>http://maven.geotoolkit.org</url>
    </repository> 
    <repository>
      <id>jmoore-java</id>
      <name>JMoore Java Lib Repo</name>
      <url>http://dl.bintray.com/jmoore/java-lib</url>
    </repository> 
</repositories>
```

Then you can use the latest version of PIXYMETA in your pom.xml:

```xml
<dependency>
  <groupId>com.mooregreatsoftware.pixymeta</groupId>
  <artifactId>pixymeta</artifactId>
  <version>{version}</version>
</dependency>
``` 


Go to the [wiki] page to see this library in action or grab the "pixymeta.jar" from the lib folder and try it yourself!

[wiki]:https://github.com/dragon66/pixymeta/wiki
[Open]:https://github.com/dragon66/pixymeta/issues/new
Suggestions? custom requirements? [Open] an issue or send email to me directly: yuwen_66@yahoo.com
