# Type_Conversions
namespace Type_Conversions;

class Program
{
    public static void Main(string[] args)
    {
        //implicit convert
        Console.WriteLine("implicit convert");
        string a = "Göktuğ";
        char b = 'a';
        byte c = 2;
        object d = a+b+c;
        Console.WriteLine("d:" + d);

        //excplicit convert
        Console.WriteLine("Explicit Convert");
        int e = 4;
        byte f = (byte)e;
        Console.WriteLine("f:" +e);

        float g = 10.2f;
        sbyte h = (sbyte)g;
        Console.WriteLine("h:" +h); // Do not forget that such conversions may result in data loss.

        //ToString Method
        Console.WriteLine("ToString Method");
        int x = 6;
        string y = x.ToString();
        Console.WriteLine("y:"+y); 

        //System Convert
        Console.WriteLine("System Convert");
        string s1 = "10", s2 = "50";
        int  i1 ,i2;
        i1 = Convert.ToInt32(s1);
        i2 = Convert.ToInt32(s2);
        int sum = i1 + i2;
        Console.WriteLine("sum:"+sum);

        //Parse
        Console.WriteLine("Parse Method");
        string k = "10";
        string l = "13.44";
        int n1;
        double d1;
        n1 = Int32.Parse(k);
        d1 = Double.Parse(l);
        Console.WriteLine("n1:"+n1);
        Console.WriteLine("d1:"+d1);
    }
}
