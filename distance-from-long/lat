import java.util.Scanner;
public class distance {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		System.out.println("please enter a latitude");
		double lat = sc.nextDouble();
		
		System.out.println("please enter a latitude");
		Scanner sc1 = new Scanner(System.in);
		double ln = sc1.nextDouble();
		
		
		//double latyork=40.6892;
		//double lonyork=-74.0444;
		double latmay=53.3846;
		double lonmay=-6.6014;
		double n=(distFrom1(lat,ln,latmay, lonmay));
		System.out.println("the distance from "+lat+","+ln+" to maynooth is "+n+"\n metres which is "+n*0.00062137+" miles");
	}
	public static double distFrom1(double lat1, double lng1, double lat2, double lng2)//method for passing in long and lat
    {
	    double earthRadius = 6371000; //meters
	    double dLat = Math.toRadians(lat2-lat1);
	    double dLng = Math.toRadians(lng2-lng1);
	    double a = Math.sin(dLat/2) * Math.sin(dLat/2) +
	               Math.cos(Math.toRadians(lat1)) * Math.cos(Math.toRadians(lat2)) *
	               Math.sin(dLng/2) * Math.sin(dLng/2);
	    double c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1-a));
	    double dist = (double) (earthRadius * c);
	
	    return dist;
    }

}
