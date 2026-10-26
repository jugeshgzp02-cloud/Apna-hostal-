
import 'package:flutter/material.dart';

void main() {
  runApp(const ApnaHostalApp());
}

class ApnaHostalApp extends StatelessWidget {
  const ApnaHostalApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Apna Hostal',
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(seedColor: Colors.green),
        useMaterial3: true,
      ),
      home: const HomePage(),
    );
  }
}

class HomePage extends StatelessWidget {
  const HomePage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('Apna Hostal'),
        backgroundColor: Colors.green,
        foregroundColor: Colors.white,
      ),
      body: Padding(
        padding: const EdgeInsets.all(16),
        child: Column(
          children: [
            const Text(
              'Apne shehar mein room khojein',
              style: TextStyle(
                fontSize: 22,
                fontWeight: FontWeight.bold,
              ),
            ),
            const SizedBox(height: 20),
            const TextField(
              decoration: InputDecoration(
                hintText: 'City ya area ka naam likhein',
                prefixIcon: Icon(Icons.search),
                border: OutlineInputBorder(),
              ),
            ),
            const SizedBox(height: 20),
            roomCard('Student Hostal', 'Ahmedabad', '₹3500/month'),
            roomCard('Apna Hostal', 'Gujarat', '₹4000/month'),
            roomCard('Sree Hostal', 'Ahmedabad', '₹4500/month'),
          ],
        ),
      ),
    );
  }

  Widget roomCard(String name, String city, String price) {
    return Card(
      child: ListTile(
        leading: const Icon(Icons.home, color: Colors.green, size: 32),
        title: Text(name),
        subtitle: Text(city),
        trailing: Text(price),
      ),
    );
  }
}
