#include <Keyboard.h>

int upStatus=1;
int upStatusPrev=1;
int leftStatus=1;
int leftStatusPrev=1;
int downStatus=1;
int downStatusPrev=1;
int rightStatus=1;
int rightStatusPrev=1;

void setup()
{
  pinMode(3,INPUT_PULLUP);
  pinMode(4,INPUT_PULLUP);
  pinMode(5,INPUT_PULLUP);
  pinMode(6,INPUT_PULLUP);
  Keyboard.begin();
}

void loop()
{
 
 upStatus=digitalRead(3);
 leftStatus=digitalRead(4);
 downStatus=digitalRead(5);
 rightStatus=digitalRead(6);
 
 //UP ARROW PRESSED
 if (upStatus!=upStatusPrev && upStatus==LOW)
 {
    Keyboard.press('w');
    upStatusPrev=upStatus;
 }
 //UP ARROW RELEASED
 if (upStatus!=upStatusPrev && upStatus==HIGH)
 {
    Keyboard.release('w');
    upStatusPrev=upStatus;
 }
 
  //LEFT ARROW PRESSED
 if (leftStatus!=leftStatusPrev && leftStatus==LOW)
 {
    Keyboard.press('a');
    leftStatusPrev=leftStatus;
 }
 //LEFT ARROW RELEASED
 if (leftStatus!=leftStatusPrev && leftStatus==HIGH)
 {
    Keyboard.release('a');
    leftStatusPrev=leftStatus;
 }
 
  //DOWN ARROW PRESSED
 if (downStatus!=downStatusPrev && downStatus==LOW)
 {
    Keyboard.press('s');
    downStatusPrev=downStatus;
 }
 //DOWN ARROW RELEASED
 if (downStatus!=downStatusPrev && downStatus==HIGH)
 {
    Keyboard.release('s');
    downStatusPrev=downStatus;
 }
 
 //RIGHT ARROW PRESSED
 if (rightStatus!=rightStatusPrev && rightStatus==LOW)
 {
    Keyboard.press('d');
    rightStatusPrev=rightStatus;
 }
 //RIGHT ARROW RELEASED
 if (rightStatus!=rightStatusPrev && rightStatus==HIGH)
 {
    Keyboard.release('d');
    rightStatusPrev=rightStatus;
 }
}
