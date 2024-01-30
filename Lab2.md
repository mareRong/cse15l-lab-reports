# Part 1
**ChatServer Code**
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    String message = "";
    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format(message);
        }

        else if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("&");
                String[] strInfo = parameters[0].split("=");
                String[] userName = parameters[1].split("=");
                message +=String.format("%s: %s \n", userName[1], strInfo[1]);
                return String.format("User %s added string %s", userName[1], strInfo[1]);
        }
        return "404 Not Found!";
        }
    }

class ChatServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
}
```

**Screenshot Result**
![image]
