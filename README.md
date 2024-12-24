import 'package:flutter/material.dart';

void main() {
  runApp(AcertijosApp());
}

class AcertijosApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'Acertijos de Navidad y Amor',
      theme: ThemeData(
        primarySwatch: Colors.red,
      ),
      home: Paso1(),
    );
  }
}

class Paso1 extends StatelessWidget {
  final TextEditingController _controller = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Paso 1'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: [
            Text(
              "Esta aplicación se creó exactamente para Anais Valentina Contreras Acevedo. Si no lo eres, se borrará automáticamente. Solo ella sabe las respuestas. Ahora escribele al amor de tu vida cómo se llaman tus mascotas.",
              style: TextStyle(fontSize: 18.0),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            TextField(
              controller: _controller,
              decoration: InputDecoration(
                labelText: 'Código',
                border: OutlineInputBorder(),
              ),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                if (_controller.text == "BIEN2023") {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => Paso2()),
                  );
                } else {
                  showDialog(
                    context: context,
                    builder: (context) => AlertDialog(
                      title: Text('Código Incorrecto'),
                      content: Text('Intenta de nuevo.'),
                      actions: [
                        TextButton(
                          onPressed: () {
                            Navigator.of(context).pop();
                          },
                          child: Text('OK'),
                        ),
                      ],
                    ),
                  );
                }
              },
              child: Text('Siguiente'),
            ),
          ],
        ),
      ),
    );
  }
}

class Paso2 extends StatelessWidget {
  final TextEditingController _controller = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Paso 2'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: [
            Text(
              "Hay lugares oscuros, por los que hemos pasado, pero quería darte gracias por sacarme de ahí. Ahora el código está en ti. Piensa y con mayúsculas, ¿qué es lo primero que comimos al conocernos?",
              style: TextStyle(fontSize: 18.0),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            TextField(
              controller: _controller,
              decoration: InputDecoration(
                labelText: 'Código',
                border: OutlineInputBorder(),
              ),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                if (_controller.text == "PIZZA") {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => Paso3()),
                  );
                } else {
                  showDialog(
                    context: context,
                    builder: (context) => AlertDialog(
                      title: Text('Código Incorrecto'),
                      content: Text('Intenta de nuevo.'),
                      actions: [
                        TextButton(
                          onPressed: () {
                            Navigator.of(context).pop();
                          },
                          child: Text('OK'),
                        ),
                      ],
                    ),
                  );
                }
              },
              child: Text('Siguiente'),
            ),
          ],
        ),
      ),
    );
  }
}

class Paso3 extends StatelessWidget {
  final TextEditingController _controller = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Paso 3'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: [
            Text(
              "Al ir conociéndonos después de ese día, el amor que tan poco quería se volvía más fuerte. De verdad tenía miedo. Este código también está en ti: ¿qué comimos ese día que nos encontramos en Miramar?",
              style: TextStyle(fontSize: 18.0),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            TextField(
              controller: _controller,
              decoration: InputDecoration(
                labelText: 'Código',
                border: OutlineInputBorder(),
              ),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                if (_controller.text == "SUSHI") {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => Paso4()),
                  );
                } else {
                  showDialog(
                    context: context,
                    builder: (context) => AlertDialog(
                      title: Text('Código Incorrecto'),
                      content: Text('Intenta de nuevo.'),
                      actions: [
                        TextButton(
                          onPressed: () {
                            Navigator.of(context).pop();
                          },
                          child: Text('OK'),
                        ),
                      ],
                    ),
                  );
                }
              },
              child: Text('Siguiente'),
            ),
          ],
        ),
      ),
    );
  }
}

class Paso4 extends StatelessWidget {
  final TextEditingController _controller = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Paso 4'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: [
            Text(
              "Las cosas se volvieron más intensas. Se que fui egoísta al pedirte exclusividad sobre todo tan rápido. Este código lo sabrás solo diciéndole algo convincente o que sentiste esos días a la persona que está a tu lado y te ama como pareja.",
              style: TextStyle(fontSize: 18.0),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            TextField(
              controller: _controller,
              decoration: InputDecoration(
                labelText: 'Código',
                border: OutlineInputBorder(),
              ),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                if (_controller.text == "ANI220") {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => Paso5()),
                  );
                } else {
                  showDialog(
                    context: context,
                    builder: (context) => AlertDialog(
                      title: Text('Código Incorrecto'),
                      content: Text('Intenta de nuevo.'),
                      actions: [
                        TextButton(
                          onPressed: () {
                            Navigator.of(context).pop();
                          },
                          child: Text('OK'),
                        ),
                      ],
                    ),
                  );
                }
              },
              child: Text('Siguiente'),
            ),
          ],
        ),
      ),
    );
  }
}

class Paso5 extends StatelessWidget {
  final TextEditingController _controller = TextEditingController();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Paso 5'),
      ),
      body: Padding(
        padding: const EdgeInsets.all(16.0),
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          children: [
            Text(
              "Son tantos los recuerdos en tan poco tiempo. Este código te lo inventas tú para pasar al último paso. Tienes 8 letras para escribir.",
              style: TextStyle(fontSize: 18.0),
              textAlign: TextAlign.center,
            ),
            SizedBox(height: 20),
            TextField(
              controller: _controller,
              decoration: InputDecoration(
                labelText: 'Código',
                border: OutlineInputBorder(),
              ),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                if (_controller.text.length == 8) {
                  Navigator.push(
                    context,
                    MaterialPageRoute(builder: (context) => Paso6()),
                  );
                } else {
                  showDialog(
                    context: context,
                    builder: (context) => AlertDialog(
                      title: Text('Código Incorrecto'),
                      content: Text('El código debe tener 8 letras.'),
                      actions: [
                        TextButton(
                          onPressed: () {
                            Navigator.of(context).pop();
                          },
                          child: Text('OK'),
                        ),
                      ],
                    ),
                  );
                }
              },
              child: Text('Siguiente'),
            ),
          ],
        ),
      ),
    );
  }
}

class Paso6 extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      app
