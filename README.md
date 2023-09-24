import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(
          leading: Icon(Icons.home),
          backgroundColor: Colors.greenAccent,
          actions: [Icon(Icons.menu)],
          title: Center(
            child: Text(
              "Project UJI COBA",
              style: TextStyle(color: Colors.black38),
            ),
          ),
        ),
        body: SingleChildScrollView(
          // Tambahkan SingleChildScrollView di sini
          child: Column(
            children: [
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg",
                title: "Playboi carti",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "Ken carson",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "Gunna",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "Lil pump",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "Juice wrld",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "xxtentacion",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "lil uzi",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "travis scot",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "kay flock",
                subtitle: "Jabatan : Rapper",
              ),
              SizedBox(height: 20),
              _buildListTile(
                imageUrl:
                    "https://i.pinimg.com/564x/f9/32/93/f932936f6c7bfdb82c41b81f21b9566c.jpg", // Ganti URL gambar
                title: "dthang",
                subtitle: "Jabatan : Rapper",
              ),
            ],
          ),
        ),
      ),
    );
  }

  Widget _buildListTile({
    required String imageUrl,
    required String title,
    required String subtitle,
  }) {
    return ListTile(
      leading: CircleAvatar(backgroundImage: NetworkImage(imageUrl)),
      title: Text(
        title,
        maxLines: 1,
        overflow: TextOverflow.ellipsis,
      ),
      subtitle: Text(
        subtitle,
        maxLines: 2,
        overflow: TextOverflow.ellipsis,
      ),
    );
  }
}
