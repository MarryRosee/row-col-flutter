# row-col-flutter
row-col-flutter
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      darkTheme: ThemeData(backgroundColor: Colors.green),
      home: Scaffold(
        backgroundColor: Colors.lightGreenAccent,
        appBar: AppBar(
          leading: Icon(
            Icons.menu,
            size: 40,
            color: Colors.deepOrange,
          ),
          actions: [
            Icon(
              Icons.shopping_bag_rounded,
              size: 40,
              color: Colors.blue,
            ),
          ],
          elevation: 36,
          backgroundColor: Colors.black,
          toolbarHeight: 70,
          centerTitle: true,
          title: Text(
            "Boutique",
            style: TextStyle(
                fontFamily: "cursive",
                fontStyle: FontStyle.italic,
                fontWeight: FontWeight.bold,
                fontSize: 30),
          ),
        ),
        body: Material(
          child: Column(
            children: [
              Expanded(
                child: Container(
                  color: Colors.pink,
                  alignment: Alignment.center,
                  child: Text("SAT"),
                ),
              ),
              Expanded(
                child: Container(
                  color: Colors.purple,
                  alignment: Alignment.center,
                  child: Text("SUN"),
                ),
              ),
              Expanded(
                child: Container(
                  color: Colors.blue,
                  alignment: Alignment.center,
                  child: Text("MON"),
                ),
              ),
              Expanded(
                child: Container(
                  color: Colors.orange,
                  alignment: Alignment.center,
                  child: Text("TUE"),
                ),
              ),
              Expanded(
                child: Container(
                  color: Colors.green,
                  alignment: Alignment.center,
                  child: Row(
                    children: [
                      Expanded(
                        child: Container(
                          color: Colors.pinkAccent,
                          alignment: Alignment.center,
                          child: Text("hello"),
                        ),
                      ),
                      Expanded(
                        child: Container(
                          color: Colors.green,
                          alignment: Alignment.center,
                          child: Text("welcome"),
                        ),
                      ),
                      Expanded(
                        child: Container(
                          color: Colors.purple,
                          alignment: Alignment.center,
                          child: Text("byebye"),
                        ),
                      ),
                    ],
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
    // Application name
  }
}
