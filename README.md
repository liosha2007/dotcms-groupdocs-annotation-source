GroupDocs Annotation for dotCMS
==============================
GroupDocs Annotation plugin for dotCMS (Source)

### Plugin Installation Instructions:

1. Download plugin from [GitHub](https://github.com/liosha2007/dotcms-groupdocs-annotation)
2. Extract files from archive to directory with name 'com.groupdocs.annotation'
3. Copy it to 'dotCMS\plugins\'
4. Open command line (with JDK 1.6)
5. Run commands `ant undeploy-plugins` , `ant build-plugins` , `ant deploy-plugins` from cms root directory

### GroupDocs Annotation plugin using:

1. Start CMS ('\bin\startup.bat')
2. Go to http://localhost/admin
3. Login (login: admin@dotcms.com  password: admin 
4. Go to 'Site Browser' -> 'Site Browser'
5. Select 'home' directory in left tree view
6. Right click by index page and click 'Open (Preview)'
7. Click to button 'Add Content'
8. Select 'Add Widget'
9. Select 'Simple Widget' -> 'Create New Simple Widget'
10. In 'Widget Title' field write any title
11. In 'Code' field write: 

	With all parameters
	```
	${GroupDocsAnnotation.RenderIframe('your_document_guid', 'document_quality', 'use_pdf', 'allow_download', 'frame_border_width', width_for_your_iframe, height_for_your_iframe)}
	```
		> * your&#95;document&#95;guid - How to get [Document ID (GUID)](http://groupdocs.com/docs/pages/viewpage.action?pageId=1409575)
		> * document&#95;quality - number 10, 20, 30...100
		> * use&#95;pdf - True or False
		> * allow&#95;download - True or False
		> * frame&#95;border&#95;width - 0 or 1
		> * width&#95;for&#95;your&#95;iframe - iframe width in pixels
		> * height&#95;for&#95;your&#95;iframe - iframe height in pixels
	Or simple:
	```
	${GroupDocsAnnotation.RenderIframe('your_document_guid', width_for_your_iframe, height_for_your_iframe)}
	```

12. Click 'Save / Publish' button (maybe you will should click 'Lock for Editing' button before)
13. Click 'Publish Page' button

How to get [Document ID (GUID)](http://groupdocs.com/docs/pages/viewpage.action?pageId=1409575)

###[Sign, Manage, Annotate, Assemble, Compare and Convert Documents with GroupDocs](http://groupdocs.com)
1. [Sign documents online with GroupDocs Signature](http://groupdocs.com/apps/signature)
2. [PDF, Word and Image Annotation with GroupDocs Annotation](http://groupdocs.com/apps/annotation)
3. [Online DOC, DOCX, PPT Document Comparison with GroupDocs Comparison](http://groupdocs.com/apps/comparison)
4. [Online Document Management with GroupDocs Dashboard](http://groupdocs.com/apps/dashboard)
5. [Doc to PDF, Doc to Docx, PPT to PDF, and other Document Conversions with GroupDocs Viewer](http://groupdocs.com/apps/viewer)
6. [Online Document Automation with GroupDocs Assembly](http://groupdocs.com/apps/assembly)

###Created by [GroupDocs Marketplace Team]( http://groupdocs.com/marketplace/ ).
