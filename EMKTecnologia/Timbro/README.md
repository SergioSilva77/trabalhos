### Regras

O combinado é executar das 19:00 até 22:00. Para não ter conflito, rodar das 19:00 até 21:00
Caso execute pela primeira vez, colocar o NSU zerado, por exemplo: 000000000000000

1. Consumo indevido
  Obter o valor da tag `xMotivo` e `dhResp` e **aguardar uma hora** após o horario `<dhResp>`
  ```xml
  <soap:Envelope
  	xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  	xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  	<soap:Body>
  		<nfeDistDFeInteresseResponse
  			xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe">
  			<nfeDistDFeInteresseResult>
  				<retDistDFeInt
  					xmlns:xsd="http://www.w3.org/2001/XMLSchema"
  					xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  					xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.01">
  					<tpAmb>1</tpAmb>
  					<verAplic>1.7.1</verAplic>
  					<cStat>656</cStat>
  					<xMotivo>Rejeicao: Consumo Indevido (Deve ser utilizado o ultNSU nas solicitacoes subsequentes. Tente apos 1 hora)</xMotivo>
  					<dhResp>2024-06-20T10:58:35-03:00</dhResp>
  					<ultNSU>000000000204555</ultNSU>
  					<maxNSU>000000000000000</maxNSU>
  				</retDistDFeInt>
  			</nfeDistDFeInteresseResult>
  		</nfeDistDFeInteresseResponse>
  	</soap:Body>
  </soap:Envelope>
  ```
