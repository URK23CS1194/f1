"""
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(
          title: Text("Patient Dashboard"),
          backgroundColor: Colors.blue,
        ),

        body: Padding(
          padding: EdgeInsets.all(16),

          child: Column(
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [

              Text(
                "Patient Information",
                style: TextStyle(
                  fontSize: 24,
                  fontWeight: FontWeight.bold,
                ),
              ),

              Text("Welcome to the Hospital Dashboard"),

              SizedBox(height: 20),

              Container(
                padding: EdgeInsets.all(15),
                margin: EdgeInsets.all(5),

                decoration: BoxDecoration(
                  color: Colors.blue.shade100,
                  borderRadius: BorderRadius.circular(15),
                ),

                child: Column(
                  crossAxisAlignment: CrossAxisAlignment.start,
                  children: [
                    Text("Patient Name: Arun"),
                    Text("Patient ID: P101"),
                    Text("Age: 35"),
                  ],
                ),
              ),

              SizedBox(height: 15),

              Row(
                mainAxisAlignment: MainAxisAlignment.spaceAround,
                children: [
                  Icon(Icons.person, size: 35),
                  Icon(Icons.medical_services, size: 35),
                  Icon(Icons.local_hospital, size: 35),
                ],
              ),

              SizedBox(height: 15),

              Card(
                child: ListTile(
                  leading: Icon(Icons.person),
                  title: Text("Assigned Doctor"),
                  subtitle: Text("Dr. Kumar"),
                ),
              ),

              Card(
                child: ListTile(
                  leading: Icon(Icons.room),
                  title: Text("Room Number"),
                  subtitle: Text("205"),
                ),
              ),

            ],
            """
          ),
        ),
      ),
    );
  }
}
