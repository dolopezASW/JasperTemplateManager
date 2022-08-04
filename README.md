# JasperTemplateManager
A project to make easier to build jasper reports

'''
Map<String, Object> params = new HashMap<>();
		params.put("nombres", "Daniel");
		params.put("apellidos", "Lopez");
		params.put("empresa", "Asesoftware");
		TemplateManager tm = new TemplateManager("C:\\JasperTemplates\\Sample01.jrxml", params);
		byte result[]=tm.buildReport(tm);
		tm.exportReportToFile(params);
		System.out.println("TERMINADO");
'''
