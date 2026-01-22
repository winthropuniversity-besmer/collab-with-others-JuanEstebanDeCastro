# collab-with-others-JuanEstebanDeCastro
Hello My name is juan I am cool
Hello Everybody, My name is Markiplier
Juan(the sigma) found an ancient city in MC
/*   
    Ryan Orjuela
    October 1st, 2025
    Programming Assignment 1: Sorting Analysis
*/
  
import java.util.*;

            System.out.println("Size, Ascending Counter\t");
            // Ascending Array
               for(int size = 1000; size <= 20000; size += 1000){
                    int[] ascArr = new
       if (mq_receive (qd_server, in_buffer, MSG_BUFFER_SIZE, NULL) == -1) {
            cerr << "Server: mq_receive";
            exit (1);
        }

        cout << "Server: message received.\n";

        // SEND REPLY MESSAGE TO CLIENT'S MAILBOX
		// The message received, contains the name of the client's mailbox.
		// That name is saved in the input buffer.

		// Open the client's mailbox
        if ((qd_client = mq_open (in_buffer, O_WRONLY)) == 1) {
            cerr << "Server: Not able to open client queue";
            continue;
        }
          // The following copies an integer (token) into the c-string that is the output buffer
		  sprintf(out_buffer, "%d", token_number);
      
        // Send the message to the client's 

 int[size]; // Input the creation of the Ascending Array to Size
                    for(int i = 0; i < size; i++) {
                        // Input of Ascending Array dicussed in class of A[i] = i
                        ascArr[i] = i;
                    }

                    // random array counter into the size from 1000-20000
                    int ascCounter = SortAnalCounter(ascArr);
                    // print
                    System.out.println(size + ", " + ascCounter);
                } 

#include <stdlib.h>
#include <string.h>
#include <sys/types.h>


#include <fcntl.h>
#include <sys/stat.h>
#include <mqueue.h>
#include <cstring>
#include <iostream>

// DEFINE THE SERVER NAME AN DEFAULT VALUES FOR THE MESSAGE QUEUE
#define SERVER_QUEUE_NAME   "/server"
#define QUEUE_PERMISSIONS 0660  // like chmod values, user and owner can read and write to queue
#define MAX_MESSAGES 10
#define MAX_MSG_SIZE 256
#define MSG_BUFFER_SIZE MAX_MSG_SIZE + 10   // leave some extra space after message

using namespace std;
/****************************************************************************
START OF MAIN PROCEDURE
This server creates a message queue an                    }
                    // random array counter into the size from 1000-20000
                    int descCounter = SortAnalCounter(descArr);
                    // print
                    System.out.println(size + ", " + descCounter);
                } 
        }   
        // results of the arrays
        catch(Exception e) {
            e.printStackTrace();
        }
    }
}
