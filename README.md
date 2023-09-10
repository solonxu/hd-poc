# hd-poc

---- add below property to the core-site.xml file 




   <property>
        <name>hadoop.http.filter.initializers</name>
        <value>org.apache.hadoop.security.AuthenticationFilterInitializer</value>
    </property>

    <property>
      <name>hadoop.http.authentication.type</name>
      <value>org.example.org.jt.hadoop.test.security.CustomizeHanlder</value>
    </property>



 <property>
      <name>hadoop.http.authentication.cust.admin.name</name>
      <value>solon,huifan</value>
    </property>


<!--   <property>
     <name>hadoop.http.authentication.signer.secret.provider</name>
     <value>file</value>
   </property>
-->
    <property>
      <name>hadoop.http.authentication.token.validity</name>
       <value>3600</value>
    </property>
   <property>
     <name>hadoop.http.authentication.signature.secret.file</name>
     <value>/home/hadoop/secret</value>
   </property>
   <property>
      <name>hadoop.http.authentication.cookie.domain</name>
      <value></value>
   </property>
   <property>
     <name>hadoop.http.authentication.simple.anonymous.allowed</name>
     <value>false</value>
   </property>

