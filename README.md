# publicTEST
testtt
 DriverManager.registerDriver(new oracle.jdbc.driver.OracleDriver());
     String url="jdbc:oracle:thin:@localhost:1521:orcl";
     String user="test_mark";
     String pass="123412312";
     String strsql="insert into STUDENT values(?,?,?)";
     Connection con=DriverManager.getConnection(url,user,pass);
     PreparedStatement ps=con.prepareStatement(strsql);
     String tid=this.jTextField3.getText();
     String tname=this.jTextField1.getText();
     String tmark=this.jTextField2.getText();
     ps.setInt(1, Integer.parseInt(tid));
     ps.setString(2, tid);
     ps.setInt(3, Integer.parseInt(tmark));
     ps.executeUpdate();
     con.commit();
     con.close();
