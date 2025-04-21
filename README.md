import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: DecorationContainerDemo(),
 );
 }
}
class DecorationContainerDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Container with Decoration')),
 body: Center(
 child: Container(
 height: 150,
 width: 150,
 decoration: BoxDecoration(
 color: Colors.blue,
 borderRadius: BorderRadius.circular(12),
 boxShadow: [
 BoxShadow(
 color: Colors.black26,
 blurRadius: 8,
 offset: Offset(4, 4),
 ),
 ],
 ),
 child: Center(
 child: Text(
 'Decorated',
 style: TextStyle(color: Colors.white, fontWeight: 
FontWeight.bold),
 ),
 ),
 ),
 ),
 );
 }
