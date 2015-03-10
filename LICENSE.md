public class CentarNaMasiv {
    static int[] array = { 10, 20, 5, 30, 40, 60, 50 };
    static int buffer1 = 0;
    static int buffer2 = 0;
    static int i;
    static int help;

    /**
     * 
     * @return
     */
    public static int Centar() {
	for (int i = 0, help = array.length - 1; i < help;) {
	    if (buffer1 < buffer2) {
		buffer1 = buffer1 + array[i++];
	    } else {
		buffer2 = buffer2 + array[help--];
	    }
	}
	System.out.println("Sbora ot parvata polovina na masiva e :" + buffer1);
	System.out.println("Sbora ot vtorata polovina na masiva e :" + buffer2);
	return i;
    }
}
