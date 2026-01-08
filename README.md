# order-pack-apphttps://github.com/rehanayanbaba-create/order-pack-app.git
Order &amp; Pack grocery app
import 'package:flutter/material.dart';

void main() {
  runApp(const OrderPackApp());
}

class OrderPackApp extends StatelessWidget {
  const OrderPackApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'Order & Pack',
      home: const HomeScreen(),
    );
  }
}

class HomeScreen extends StatelessWidget {
  const HomeScreen({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: const Text('Order & Pack')),
      body: Padding(
        padding: const EdgeInsets.all(16),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.start,
          children: const [
            Text(
              'Select items and press Order & Pack',
              style: TextStyle(fontSize: 18),
            ),
            SizedBox(height: 20),
            Text('• Rice'),
            Text('• Milk'),
            Text('• Biscuits'),
            Text('• Vegetables'),
            Spacer(),
            Center(
              child: Text(
                'Pickup time: 4–5 seconds',
                style: TextStyle(
                    color: Colors.green,
                    fontWeight: FontWeight.bold),
              ),
            )
          ],
        ),
      ),
    );
  }
}
Add main Flutter app file
