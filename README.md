# mi-app
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  get fontSize => null;




  @override
  Widget build(BuildContext context) {
    return   const MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.teal,
      
      body: SafeArea(
        child:Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
             CircleAvatar(
              radius: 50,
              backgroundImage: AssetImage('images/abhinav.jpg'),
            ),
            Text('Abhinav',
             style:TextStyle(
               fontFamily: 'Pacifico',
               fontSize:40,
               color: Colors.white,
               fontWeight: FontWeight.bold,
            ),
            ),
            Text('FLUTTER DEVELOPER',
            style:TextStyle(
              fontFamily: 'SourceCodePro',
              fontSize: 20,
              color: Colors.white,
              letterSpacing: 2.5,
              fontWeight: FontWeight.bold,
            ),
            ),
       SizedBox(
         height: 20,
         width: 100,
         child: Divider(
           color: Colors.black,
         ),
       ),
       Card(

           margin: EdgeInsets.symmetric(horizontal: 25,vertical: 20),
           child: ListTile(
             leading: Icon(
               Icons.email,
               color: Colors.black,
             ),
             title: Text('abhinavsajiv89@gmail.com',
             style:TextStyle(
           color: Colors.black,
           fontFamily: 'Pacifico',
           fontSize: 20,
             ),
           ),
           ),
         ),
              Card(

                margin: EdgeInsets.symmetric(horizontal: 25,vertical: 20),
                child: ListTile(
                  leading:Icon(
                    Icons.phone,
                    color: Colors.black,
                  ),
                  title: Text('7306655228',
                    style: TextStyle(
                      color: Colors.black,
                      fontFamily: 'Pacifico',
                      fontSize: 20,
                    ),

                  ),
                )
              ),

          ],

        ),
      ),),
    );
  }
}
