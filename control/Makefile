
# checks only those control files that belong to this package
check: /usr/share/YaST2/control/control.rng
	xmllint --relaxng /usr/share/YaST2/control/control.rng --noout *.xml

# generate the control.TWKubic.xml file
control.Kubic.xml: control.Kubic.xsl control.Kubic.xml
	xsltproc control.Kubic.xsl control.Kubic.xml > control.TWKubic.xml

clean:
	rm -f control.Kubic.xml
