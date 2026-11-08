
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Patient Dashboard"),
        ),

        body: Column(
          children: [

            Text("Patient Information"),

            Container(
              padding: EdgeInsets.all(10),
              color: Colors.blue.shade100,
              child: Column(
                children: [
                  Text("Name: Arun"),
                  Text("ID: P101"),
                  Text("Age: 35"),
                ],
              ),
            ),

            Row(
              mainAxisAlignment: MainAxisAlignment.spaceEvenly,
              children: [
                Icon(Icons.person),
                Icon(Icons.local_hospital),
                Icon(Icons.medical_services),
              ],
            ),

            Card(
              child: ListTile(
                title: Text("Assigned Doctor"),
                subtitle: Text("Dr. Kumar"),
              ),
            ),

            Card(
              child: ListTile(
                title: Text("Room Number"),
                subtitle: Text("205"),
              ),
            ),

          ],
        ),
      ),
    );
  }
}
