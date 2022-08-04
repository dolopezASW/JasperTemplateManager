# JasperTemplateManager
A project to make easier to build jasper reports

# Example
In the next example we see an example for passing params for a template that we pass the name too.
params is the map with the values for fill the template.
TemplateManager take the path + template name joined in one string as parameter and create a new instance with thye template jrxml provided.
the method buildReport generate the report from the jrxml template.
exportReportToFile receive the params and generate the pdf file and exported to project folder.

```java
Map<String, Object> params = new HashMap<>();
		params.put("nombres", "Daniel");
		params.put("apellidos", "Lopez");
		params.put("empresa", "Asesoftware");
		TemplateManager tm = new TemplateManager("C:\\JasperTemplates\\Sample01.jrxml", params);
		byte result[]=tm.buildReport(tm);
		tm.exportReportToFile(params);
```
