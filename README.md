R. fractured lateral tibial condyle
================================

##STL object info
- **r_fractured_lateral_condyle-inner_removed-P01.stl** is the primary 3D printable object.
- **r_fractured_lateral_condyle-inner_removed.stl** is an intermediate-stage, reference STL as generated by Invesalius.

##Production notes
###Workflow
1. DICOM format CT scan data was converted to STL mesh using the open source software [Invesalius](http://www.cti.gov.br/invesalius/) [v3.0b1](http://svn.softwarepublico.gov.br/trac/invesalius/wiki/downloads/3.0-beta-1).

 **Note:** Three other DICOM -> STL conversion tools, (ImageJ, Slicer and InVesalius v3.0b3) all crashed while trying to generate the mesh. Useable output was only achieved with InVesalius 3.0b1.

2. Due to the complex non-manifoldness of the Invesalius generated STL, it was used instead as reference for reconstructing a manifold mesh using (free) [MeshMixer 08](http://www.meshmixer.com/). In particular, the pull (to reference geometry) tool was the most efficient way to match the new mesh to the reference STL, and enable filling in of the very many missing gaps.

###Total project time
- A week of finding, experimenting and learning new tools,
- 4 to 6 hours 'actual' productivity (after dicovering the MeshMixer pull tool),
- 3 hours printing at slow speed (40mm/s) with single wall and 15% infill.

3D print as shown in images was sliced at 0.2mm layer height using Slic3r 0.9.5. It was printed at 40mm/s on a Prusa Mendel fitted with a J-Head Mk IV-B hotend.

##First Printed
2012-11-17

##Inspiration and guidance
[3D Printing For CT Scan Analysis, Space Education](http://makezine.com/2012/05/01/3d-printing-improves-ct-scan-analysis-space-education/)

##License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">fractured-lateral-tibial-condyle</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/hairykiwi/fractured-lateral-tibial-condyle/" property="cc:attributionName" rel="cc:attributionURL">Hamish Mead</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.

