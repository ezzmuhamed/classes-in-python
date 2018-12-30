
"""
 we should defined this variable in our main program
 PPR  = 250                                                                           // Pulses per Revolution
 SAMPLETIME = 10                                                                     // a milliSeconds SampleTime 
 minuteInMillis = 60000                                                              // A minute represented in milli seconds
 PPCM = (PPR / (3.14 * 5 * 2.54))                                                    // Pulses generated from encoders per cm 
 MAX_SPEEDS = 20                                                                     // Maximum stored speeds in Motor Array
 MOTOR_SPEED_STEP = 24                                                               // Motor speeds steps 
 FACTOR = 1.74
 rotconstant = (0.25 * 3.14 * 56 )
 rotconstant90 = (0.23 * 3.14 * 56 )
 rotconstant0 =(0.3 * 3.14 * 56 )
 plaunch = 11
 dlaunch = 10
  // For determining motor rotating direction 
 COUNTER_CLOCK_WISE = 1                    
 CLOCK_WISE = 0

"""
class Motor(object):

   
    def __init__(self,dpin = None,spin = None,data= None):
        motorSpeedsArray = []
        self.directioPin = dpin ;
        self.pwmPin = spin ;
        self.motorSpeedsArray = data ;
        """
        I need few element of array
        for i in range(11):
            motorSpeedsArray.append(data[i])
        self.motorSpeedsArray_2 = motorSpeedsArray;    
        """
        self.motorSpeed = 0;
        self.distanceTravelled = 0.0;
        self.pulseCount = 0;

       
    def __repr__(self):
      self.motorSpeed = 0;
      self.distanceTravelled = 0.0;
      self.pulseCount = 0;
      self.MOTOR_SPEED_STEP = 24
      
      
    def __repr__(self,dpin=None,spin=None):
        self.directioPin = dpinn ;
        self.pwmPin = spinn ;
        self.motorSpeed = 0;
        self.distanceTravelled = 0.0;
        self.pulseCount = 0;
        self.MOTOR_SPEED_STEP = 24;
    
    """
      This is three constructor we can take instance from it by give it
      special parameters to each constructor
    """
    #now we make methods to this class.
    
    def movement(self, velocity, direct):
        motorDirection = direct;
        self.directionPin =  motorDirection ;
        self.pwmPin = self.motorSpeedsArray[(velocity // MOTOR_SPEED_STEP) - 2];

    def movement_2(self, velocity, direct, distance):
      motorDirection = direct ;
      self.directionPin = motorDirection ; 
      self.pwmPin =  self.motorSpeedsArray[(velocity // MOTOR_SPEED_STEP) - 2];
      while(distanceTravelled < distance):
          self.pwmPin = 0 ;

    def movement_3(self):
        self.pwmPin = 0 ;

    def Move(velocity,direct):
        motorDirection = direct;
        self.directionPin = motorDirection;
        self.pwmPin = velocity ;
        
    def pulseIncrement(self):
        self.pulseCount += 1
        
    """
      Don't need seter and geter function as c & c++ beacause we can modify
      by name.pulsecount = 10 this we put in it value when need to return it
      name.pulsecount and then enter return 10
    """
    def measure (self):
        self.motorSpeed = (self.pulseCount * minuteInMillis) / (SAMPLETIME * PPR);
        self.distanceTravelled += self.pulseCount / PPCM;
        self.pulseCount = 0;
    def getData(self):
        
        print(self.directioPin,"  ",self.pwmPin,"  ",self.motorSpeedsArray)
        
class Robot(Motor):
    
     def __init__(self,Mot1,Mot2,Mot3,Mot4):
         self.MotA =  Mot1
         self.MotB =  Mot2
         self.MotC =  Mot3
         self.MotD =  Mot4
         
         self.dA = 0;
         self.dB = 0;
         self.dC = 0;
         self.dD = 0;
         



     def stopMovement(self):
         self.MotA.movement_3()
         self.MotB.movement_3()
         self.MotC.movement_3()
         self.MotD.movement_3()
         

     def movementation(self, v, a, d):
         while(self.dA <= d | self.dB <= d | self.dC <= d | self.dD <= d):
             if(a==0):
                 MotA.movement(v, COUNTER_CLOCK_WISE);
                 MotB.movement(v, COUNTER_CLOCK_WISE);
                 MotC.movement(v, COUNTER_CLOCK_WISE);
                 MotD.movement(v, COUNTER_CLOCK_WISE);
                 break;
             elif(a==90):
                 MotA.movement(self,v, CLOCK_WISE);
                 MotB.movement(self,v, COUNTER_CLOCK_WISE);
                 MotC.movement(self,v, COUNTER_CLOCK_WISE);
                 MotD.movement(self,v, CLOCK_WISE);
                 break;
             elif(a==180):
                 MotA.movement(self,v, CLOCK_WISE);
                 MotB.movement(self,v, CLOCK_WISE);
                 MotC.movement(self,v, COUNTER_CLOCK_WISE);
                 MotD.movement(self,v, COUNTER_CLOCK_WISE);
                 break;
             elif(a==270):
                 MotA.movement(self,v, COUNTER_CLOCK_WISE);
                 MotB.movement(self,v, CLOCK_WISE);
                 MotC.movement(self,v, CLOCK_WISE);
                 MotD.movement(selfv, COUNTER_CLOCK_WISE);
                 break;



    
        

    



