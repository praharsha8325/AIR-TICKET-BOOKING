# AIR-TICKET-BOOKING
#include<stdio.h>


void info();
void booking ();

void main()
    {
	int option;
	printf("\n\t\t\t\t\t WELCOME TO AIR TICKECT BOOKING SYSTEM");
	printf("\n 1.INFORMATION \n 2.BOOKING\n\n");
	scanf("%d",&option);
	switch(option)
	{
	
		case 1:
			info();
			break;
		case 2:
		    booking();
			break;
		default:
		printf("\n ENTER A VALID OPTION \n");
		main();
			
			
	}
}
void info()
{
printf("\t\t\t\t\t\t*INFORMATION*\nTHIS IS A LIST OF AIRLINES OF INDIA OPERATING IN THE AREA OF CIVIL AVIATION..\n1.JET AIRWAYS(The Jet Airways is the second largest airline in India with a market share of 15.4 percent. It was established on 1st April, 1992 and started operations on 5th May, 1993. Chhatrapati Shivaji International Airport, Mumbai is the main hub of Jet Airways.)\n2.AIR INDIA(Air India is one of the oldest airline companies in India with presence in all the major as well as small cities of India. It was founded in July, 1930 as the Tata Airlines and started operations on 15th October, 1932. The airline was founded by one of the great industrialists JRD Tata.)\n3.SPICEJET(The SpiceJet Airlines serves in key cities of India such as Pune, Chennai, Ahmedabad, Goa and so on. Previously, it was owned by the NRI group and it was acquired by the media king Kalanithi Maran. However, Maran sold his shares back to Ajay Singh in 2015.)\n4.GOAIR(GoAir is the one of the most popular budget airlines in India. GoAir is promoted by the Wadia Group. It was founded in 2005 and started operations in November, 2005. The fleet size of the GoAir is 38 aircraft and serves in more than 23 destinations. The GoAir is headquartered in Worli, Mumbai, Maharashtra with the slogan of “Fly Smart”.)\n");
return;
}
void booking()
{
int option1,option2,passengers,price,class,d=002;
char route;
rout:
 printf("\t\t\t\t\t***CHOOSE  YOUR ROUTE** \n");
 printf("A.INTERNATIONAL \nOR\nB.NATIONAL\n");
 scanf("%c",&route);
 if(route==65||route==97)
 {
  OPTION:
 printf("\t\t\t\t\t**INTERNATIONAL ROUTES** \n1.AUSTRALIA\n2.USA\n3.CANNADA\n4.SWITZERLAND\n\n");
 scanf("%d",&option1);
 if (option1<=4)
 {
  clas:
 printf("\t\t\t\t\t**CHOOSE YOUR CLASS**\n1.1ST CLASS\n2.2ND CLASS\n3.3RD CLASS\n");
 scanf("%d",&class);
 {
 switch(class)
 {
  case 1:
  class =5000;
  printf("------------YOU HAVE CHOOSEN CLASS 1-----------\n");
  break;
  case 2:
  class =3000;
  printf("------------YOU HAVE CHOOSEN CLASS 2----------\n");
  break;
  case 3:
  class =2000;
  printf("------------YOU HAVE CHOOSEN CLASS 3-----------\n");
  break;
  default:
  printf("CHOOSE YOUR CLASS AGAIN\n");
  goto clas;
 }
  {
  
  printf("\t\t***ENTER NUMBER OF PASSENGERS***\n");
  scanf("%d",&passengers);
}
  {
   switch(option1)
   {
  	case 1:
	 price=passengers*(10000+class);
	 printf("YOU HAVE CHOSEN TICKET FROM INDIA TO AUSTRALIA\n");
 	 printf("THE COST OF THIS TICKET IS 10000\n ");
	 printf("THE TICKET PRICE FOR %d MEMBERS IS %d\n",passengers,price);
	 break; 
	case 2: 
	 price=passengers*(15000+class);
	 printf("YOU HAVE CHOSEN TICKET FROM INDIA TO USA \n");
	 printf("THE COST OF THIS TICKET IS 15000 \n");
	 printf("THE TICKET PRICE FOR %d MEMBERS IS %d\n",passengers,price);
	 break;
	case 3:
	 price=passengers*(15000+class);
	 printf("YOU HAVE CHOSEN TICKET FROM INDIA TO CANNADA\n");
	 printf("THE COST OF THIS TICKET IS 15000 \n");
	 printf("THE TICKET PRICE FOR %d MEMBERS IS %d\n",passengers,price);
	 break; 
	case 4:
	 price=passengers*(20000+class);
	 printf("YOU HAVE CHOSEN TICKET FROM INDIA TO SWITZERLAND\n");
	 printf("THE COST OF THIS TICKET IS 20000\n ");
	 printf("THE TICKET PRICE FOR %d MEMBERS IS %d\n",passengers,price);
	 break; 
	 default:
	  printf("PLEASE RE-CHOOSE YOUR OPTIONS\n");
  } 
  }
  }
  }
   else 
   {
   printf("PLEASE RE CHOOSE YOUR OPTIONS\n");
   goto OPTION;
  }
  }
 else if (route==66||route==98)
 {
 nat:
{
 printf("\t\t\t\t\t\t**NATIONAL ROUTES*** \n1.HYDERABAD TO BENGALURU\n2.HYDERABAD TO CHENNAI\n3.HYDERABAD TO DELHI\n4.HYDERABAD TO VIZAG/VISHAKAPATNAM\n5.HYDERABAD TO GOA\n");
 scanf("%d",&option2);
 if (option2<=5)
{
 classs :
  printf("\t\t\t\t\t**CHOOSE YOUR CLASS**\n1.1ST CLASS\n2.2ND CLASS\n3.3RD CLASS\n");
 scanf("%d",&class);
 switch(class)
 {
  case 1:
  class =5000;
  printf("YOU HAVE CHOOSEN CLASS 1\n");
  break;
  case 2:
  class =3000;
  printf("YOU HAVE CHOOSEN CLASS 2\n");
  break;
  case 3:
  class =2000;
  printf("YOU HAVE CHOOSEN CLASS 3\n");
  break;
  default:
  printf("CHOOSE YOUR CLASS AGAIN\n");
  goto classs;
 }
 {
 printf("\t\t***ENTER NUMBER OF PASSENGERS***\n");
 scanf("%d",&passengers);
 }
 switch(option2)
 {
 case 1:
 price = passengers*(4000+class);
 printf("YOU HAVE CHOSEN TICKET FROM HYDERABAD TO BENGALURU\n");
 printf("THE COST OF THIS TICKET IS 4000 \n");
 printf("THE TOTAL TICKET PRICE FOR HYDERABAD TO BENGALURU FOR %d MEMBERS IS %d \n",passengers,price);
 break;
 case 2:
 price = passengers*(5000+class);
 printf("YOU HAVE CHOSEN TICKET FROM HYDERABAD TO CHENNAI\n");
 printf("THE COST OF THIS TICKET IS 5000\n ");
 printf("THE TOTAL TICKET PRICE FOR HYDERABAD TO CHENNAI FOR %d MEMBERS IS %d\n",passengers,price);
 break;
 case 3:
 price = passengers * (6000+class);
 printf("YOU HAVE CHOSEN TICKET FROM HYDERABAD TO DELHI\n");
 printf("THE COST OF THIS TICKET IS 6000 \n");
 printf("THE TOTAL TICKET PRICE FOR HYDERABAD TO DELHI FOR %d MEMBERS IS %d \n",passengers,price);
 break;
 case 4:
 price = passengers * (3000+class);
 printf("YOU HAVE CHOSEN TICKET FROM HYDERABAD TO VIZAG/VISHAKAPATNAM\n");
 printf("THE COST OF THIS TICKET IS 3000 \n");
 printf("THE TOTAL TICKET PRICE FOR HYDERABAD TO VIZAG/VISHAKAPATNAM FOR %d MEMBERS IS %d \n",passengers,price);
 break;
 case 5:
 price = passengers * (4000+class);
 printf("YOU HAVE CHOSEN TICKET FROM HYDERABAD TO GOA\n");
 printf("THE COST OF THIS TICKET IS 4000 \n");
 printf("THE TOTAL TICKET PRICE FOR HYDERABAD TO GOA FOR %d MEMBERS IS %d \n",passengers,price);
 break;
 default:
 printf("PLEASE RE-ENTER YOUR OPTION \n");
 }
}
else 
{
 printf("PLEASE CHOOSE YOUR OPTIONS\n");
 goto nat;
}
}
}
 else
{
  printf("PLEASE CHOOSE YOUR ROUTE\n");
  goto rout;
return;
}
printf("\t\t\t\t\t\t * THANK YOU \t\t\t\t\t\t\n \t\t\t\t\t\t*VISIT AGAIN\t\t\t\t\t\t ");
}
