# Draw_shapes
This program helps you to draw geometric shapes.
Kadir Pekdemir

public static void main(String[] args) {
			 
			
			int infinity = 0;
			//loop ends when only '6' is written
			while (infinity != 1) {
			
			//Create a Scanner
			Scanner input = new Scanner(System.in);
			//Ask the user what they want to draw
			System.out.println("Which shape would you like to draw?");
			System.out.println("1.Line\n2.Triangle\n3.Rectangle\n4.Parabola\n5.Circle\n6.Exit");
			  //Get selection from user
		      int choice = input.nextInt();
		      //Assign variables
		      int a,b,c,d,e,f,r;
		      
		      switch(choice) {
		      //if user presses 1
		       case 1:
		   		System.out.println("Line formula is y = ax + b\nPlease enter the coefficients a and b:");
		   		//get a and b values from user
		   		a = input.nextInt();
		   		b = input.nextInt();
		   		//run line method
		   		line(a,b);
		   		break;
		   	  //if user presses 2
		       case 2:
		    	   System.out.println("For triangle, we need the coordinates of the points for three vertices.\nPlease enter the coordinates of 3 vertices a, b, c, d, e, f:");
		    	   //get a, b, c, d, e and f values from user
			   		a = input.nextInt();
			   		b = input.nextInt();
			   		c = input.nextInt();
			   		d = input.nextInt();
			   		e = input.nextInt();
			   		f = input.nextInt();
			   	//run triangle method
			   		triangle(a,b,c,d,e,f);
			   		break; 
			   //if user presses 3
		       case 3:
		    	   System.out.println("For rectangle, we need the coordinates of the points for three vertices.\nPlease enter the coordinates of 3 vertices a, b, c, d, e, f:"); 
		    	 //get a, b, c, d, e and f values from user
		    	    a = input.nextInt();
			   		b = input.nextInt();
			   		c = input.nextInt();
			   		d = input.nextInt();
			   		e = input.nextInt();
			   		f = input.nextInt();
			   	//run rectangle method
			   		rectangle(a,b,c,d,e,f);
			   		break;
			   //if user presses 4
		       case 4:
		    	   System.out.println("Parabola formula is y = ax^2 + bx + c\nPlease enter the coefficients a, b and c:");
		    	 //get a, b and c values from user
		    	   a = input.nextInt();
		    	   b = input.nextInt();
		    	   c = input.nextInt();
		    	 //run parabola method
		    	   parabola(a,b,c);
		    	   break;
		       //if user presses 5  
		       case 5:
		    	   System.out.println("Circle formula is (x-a)^2 + (y-b)^2 = r^2\nPlease enter the coordinates of the center (a,b) and the radius:");
		    	 //get a, b and r values from user
		    	   a = input.nextInt();
		    	   b = input.nextInt();
		    	   r = input.nextInt();
		    	 //run circle method
		    	   circle(a,b,r);
		    	   break;
		    	//if user presses 6   
		       case 6:
		    	   infinity++;
		    	   break;
		    	   
		    	   	   
		    	   	   
		      }
		    
			}
		    
			
		}


}
