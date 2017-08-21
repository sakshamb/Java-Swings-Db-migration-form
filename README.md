# Java-Swings-Db-migration-form
this code is for a db to db migrator portal.. the code is just for the front end of the portal and is developed using java swings
	private Element getNodeElement(NodeList nodeList, String nodeName) {
		
		if (nodeList != null && nodeList.getLength() > 0) {
			for (int i = 0; i < nodeList.getLength(); i++) {
				if (nodeList.item(i).getNodeType() == Node.ELEMENT_NODE) {
					Element element = (Element) nodeList.item(i);
					if (element.getNodeName().equals(nodeName)) {
						return element;
					} else {
						  getNode1Element(element.getChildNodes(), nodeName);
					}
				}
			}
		}
	}
	

	public static void main(String[] args) {
		BPMNUtil utils = new BPMNUtil();
		Map<String, String> att = new HashMap<>();
		att.put("fill", "green");
		String xml = "<?xml version=\"1.0\" encoding=\"UTF-8\"?> \n"
				+ "<bpmn:definitions xmlns:bpmn=\"http://www.omg.org/spec/BPMN/20100524/MODEL\" xmlns:bpmndi=\"http://www.omg.org/spec/BPMN/20100524/DI\" xmlns:dc=\"http://www.omg.org/spec/DD/20100524/DC\" xmlns:di=\"http://www.omg.org/spec/DD/20100524/DI\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" id=\"Definitions_1\" targetNamespace=\"http://bpmn.io/schema/bpmn\"><bpmn:collaboration id=\"Collaboration_089ejrd\"><bpmn:participant id=\"Participant_1q4k7zn\" name=\"BPMN Template\" processRef=\"Process_0t4bcwn\" /></bpmn:collaboration><bpmn:process id=\"Process_0t4bcwn\"><bpmn:startEvent id=\"StartEvent_19dv59s\" name=\"START\"><bpmn:outgoing>SequenceFlow_0uikj48</bpmn:outgoing></bpmn:startEvent><bpmn:endEvent id=\"EndEvent_1p39nl8\" name=\"END\"><bpmn:incoming>SequenceFlow_067ewbm</bpmn:incoming></bpmn:endEvent><bpmn:sequenceFlow id=\"SequenceFlow_0uikj48\" sourceRef=\"StartEvent_19dv59s\" targetRef=\"WT_452794\" /><bpmn:sequenceFlow id=\"SequenceFlow_1hpw6ap\" sourceRef=\"WT_452794\" targetRef=\"WT_452795\" /><bpmn:sequenceFlow id=\"SequenceFlow_067ewbm\" sourceRef=\"WT_452795\" targetRef=\"EndEvent_1p39nl8\" /><bpmn:userTask id=\"WT_452795\" name=\"ALM\"><bpmn:incoming>SequenceFlow_1hpw6ap</bpmn:incoming><bpmn:outgoing>SequenceFlow_067ewbm</bpmn:outgoing></bpmn:userTask><bpmn:userTask id=\"WT_452794\" name=\"ALM\"><bpmn:incoming>SequenceFlow_0uikj48</bpmn:incoming><bpmn:outgoing>SequenceFlow_1hpw6ap</bpmn:outgoing></bpmn:userTask></bpmn:process><bpmndi:BPMNDiagram id=\"BPMNDiagram_1\"><bpmndi:BPMNPlane id=\"BPMNPlane_1\" bpmnElement=\"Collaboration_089ejrd\"><bpmndi:BPMNShape id=\"Participant_1q4k7zn_di\" bpmnElement=\"Participant_1q4k7zn\"><dc:Bounds x=\"270\" y=\"76\" width=\"861\" height=\"252\" /></bpmndi:BPMNShape><bpmndi:BPMNShape id=\"StartEvent_19dv59s_di\" bpmnElement=\"StartEvent_19dv59s\"><dc:Bounds x=\"316\" y=\"179\" width=\"36\" height=\"36\" /><bpmndi:BPMNLabel><dc:Bounds x=\"316\" y=\"215\" width=\"35\" height=\"12\" /></bpmndi:BPMNLabel></bpmndi:BPMNShape><bpmndi:BPMNShape id=\"WT_452794_di\" bpmnElement=\"WT_452794\"><dc:Bounds x=\"484\" y=\"157\" width=\"100\" height=\"80\" /></bpmndi:BPMNShape><bpmndi:BPMNShape id=\"EndEvent_1p39nl8_di\" bpmnElement=\"EndEvent_1p39nl8\"><dc:Bounds x=\"989\" y=\"179\" width=\"36\" height=\"36\" /><bpmndi:BPMNLabel><dc:Bounds x=\"995\" y=\"215\" width=\"23\" height=\"12\" /></bpmndi:BPMNLabel></bpmndi:BPMNShape><bpmndi:BPMNEdge id=\"SequenceFlow_0uikj48_di\" bpmnElement=\"SequenceFlow_0uikj48\"><di:waypoint xsi:type=\"dc:Point\" x=\"352\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"411\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"411\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"484\" y=\"197\" /><bpmndi:BPMNLabel><dc:Bounds x=\"426\" y=\"197\" width=\"0\" height=\"0\" /></bpmndi:BPMNLabel></bpmndi:BPMNEdge><bpmndi:BPMNEdge id=\"SequenceFlow_1hpw6ap_di\" bpmnElement=\"SequenceFlow_1hpw6ap\"><di:waypoint xsi:type=\"dc:Point\" x=\"584\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"653\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"653\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"807\" y=\"197\" /><bpmndi:BPMNLabel><dc:Bounds x=\"668\" y=\"197\" width=\"0\" height=\"0\" /></bpmndi:BPMNLabel></bpmndi:BPMNEdge><bpmndi:BPMNShape id=\"WT_452795_di\" bpmnElement=\"WT_452795\"><dc:Bounds x=\"807\" y=\"157\" width=\"100\" height=\"80\" /></bpmndi:BPMNShape><bpmndi:BPMNEdge id=\"SequenceFlow_067ewbm_di\" bpmnElement=\"SequenceFlow_067ewbm\"><di:waypoint xsi:type=\"dc:Point\" x=\"907\" y=\"197\" /><di:waypoint xsi:type=\"dc:Point\" x=\"989\" y=\"197\" /><bpmndi:BPMNLabel><dc:Bounds x=\"948\" y=\"182\" width=\"0\" height=\"0\" /></bpmndi:BPMNLabel></bpmndi:BPMNEdge></bpmndi:BPMNPlane></bpmndi:BPMNDiagram></bpmn:definitions>";
		utils.addAttribute("bpmndi:BPMNShape", att, "453123", xml);
	}
