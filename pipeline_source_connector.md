## &#9724; Source DB 설정
데이터가 쓰여질 데이터베이스를 선택합니다. 선택된 데이터베이스의 테이블로부터 이벤트 스트림이 만들어지고, 
데이터 파이프라인의 소스가 됩니다. 

+ Source Database 선택 : 데이터베이스 인스턴스를 선택합니다.
+ 테이블 선택 : 파이프라인 소스로 사용될 테이블을 선택합니다.
+ 스키마 전송 유형 : 스키마 레지스트리는 이벤트 스트림에 쓰여지는 데이터베이스의 데이터가 어떤 스키마로 정의되어 있는지를 별도로 저장하여 관리합니다. 스키마 레지스트리를 사용하지 않으면 이벤트 스트림 데이터에 스키마 정보가 쓰여지게 되어 이벤트 데이터의 용량이 늘어나게 됩니다.
  ```
  스키마 레지스트리가 backing service에 등록되지 않은 경우 스키마 레지스트리를 사용할 수 없습니다. 
  ```
+ 데이터 전송 유형 : 데이터를 텍스트 형태의 JSON으로 보낼지, 바이너리 형태로 보낼지(AVRO)를 선택합니다.
  ```
  바이너리 형태는 반드시 스키마 레지스트리를 사용하여야 하며, 스키마 레지스트리를 선택하지 못하는 경우 텍스트(JSON) 유형만 선택 가능합니다.
  ```
