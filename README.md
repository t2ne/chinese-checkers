# Chinese Checkers ♟️  
A JavaFX-based Chinese Checkers game with client-server communication and bot support. Developed as part of an academic project in the Programming Lab course.

---

## 🌟 Features

- **Multiplayer Support**: Play with others on the same network by connecting a client to a host running the server.
- **Bot Integration**: Play solo against computer-controlled players.
- **Client-Server Architecture**: Separate server and client modules for modular communication.
- **JavaFX Interface**: Interactive game UI built using JavaFX 21.

---

## 🛠️ Installation

### Requirements:
- Java 21
- OpenJFX 21 (LTS)
- IntelliJ IDEA (recommended, since the project was developed with it)

---

### Clone the repository:
```bash
git clone https://github.com/t2ne/chinese-checkers.git
```

---

### Setup Instructions (IntelliJ)

1. Open the project in IntelliJ IDEA.
2. Go to `Run` -> `Edit Configurations`.
3. Create **two new Application configurations**:
   - Name them `Run Server` and `Run Client`.
   - For **both configurations**:
     - Set the **Main Class** to `run.Run`
     - Set the **JDK** to **Java 21**
   - For the **Run Server**, select the **`server` module**
   - For the **Run Client**, select the **`client` module**

4. Go to `Modify Options` → `Add VM Options` and add the **JavaFX module paths** as shown below (adjust to your system):

#### Example VM Options:

**Machine 1:**
```
--module-path C:\Users\t2ne\.m2\repository\org\openjfx\javafx-controls\21;C:\Users\t2ne\.m2\repository\org\openjfx\javafx-fxml\21;C:\Users\t2ne\.m2\repository\org\openjfx\javafx-graphics\21;C:\Users\t2ne\.m2\repository\org\openjfx\javafx-base\21 --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.base
```

**Machine 2:**
```
--module-path C:\Users\eduko\.m2\repository\org\openjfx\javafx-controls\21;C:\Users\eduko\.m2\repository\org\openjfx\javafx-fxml\21;C:\Users\eduko\.m2\repository\org\openjfx\javafx-graphics\21;C:\Users\eduko\.m2\repository\org\openjfx\javafx-base\21 --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.base
```

5. Click **Apply** and **OK** to save.

---

### Running the Project

- Start the **Server** using the `Run Server` configuration.  
  If the terminal displays `"LOOP"`, the server is running successfully.
- Start the **Client** using the `Run Client` configuration.  
  If the GUI window opens correctly, the client is functioning.

> To play with others, one player must run the server, and others on the same network can connect via client.

> If you prefer to play alone, you can play against built-in bots.

---

## 🌐 Supported Platforms

Tested on:

- Windows (JavaFX 21 setup required)
- Linux and macOS (with appropriate JavaFX setup)

---

## 🙋‍♂️ Author

[@t2ne](https://github.com/t2ne) - [@eduardoc0uto](https://github.com/eduardoc0uto) - [@DPinto20](https://github.com/DPinto20) 

---

## 🎓 Academic Project

This game was developed as part of a university assignment in the **Programming Lab** course. It demonstrates the use of JavaFX for UI, Java modular architecture, and client-server communication for multiplayer gameplay.
