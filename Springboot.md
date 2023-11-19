## build spring don't use 'mvn'

./mvnw -N io.takari:maven:wrapper 

./mvnw install -DskipTests      : Sử dụng Maven để xây dựng ứng dụng, và -DskipTests bỏ qua việc chạy các bài kiểm thử.

./mvnw clean install


## run project with '-jar'
- in appllication.properties: 
  + server.servlet.context-path=/hysteryale
- run:  java -jar file.war
