using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace MODUL3_1302194043
{
    class Program
    {
        static void Main(string[] args)
        {
            KodeBuah table_Kodebuah = new KodeBuah();
            Console.WriteLine("=== GET KODE BUAH===");
            table_Kodebuah.getKodebuah("Apel");
            Console.WriteLine("==== GET ALL KODE BUAH ====");
            table_Kodebuah.getAllkodebuah();

            Console.WriteLine(" ");
            Console.WriteLine("================== POSISI LANDING ================");
            PosisiKarakterGame jongkok = new PosisiKarakterGame();
            jongkok.jongkok();


        }

    }
    class KodeBuah
    {

        Dictionary<string, string> dic = new Dictionary<string, string>() {
            {"Apel", "A00"},
            {"Aprikot","B00" },
            {"Alpukat"  ,"C00" },
            {"Pisang"    ,"D00" },
            {"Paprika"  ,"E00"},
            {"Blackberry" ,"F00" },
            {"Ceri","H00"},
            {"Kelapa" ,"I00" },
            {"Jagung","J00"},
            {"Kurma"   ,"K00"},
            {"Durian"   ,"L00"},
            {"Anggur"   ,"M00"},
            {"Melon"   ,"N00"},
            {"Semangka"   ,"O00"},};

        public void getKodebuah(string kel)
        {

            if (dic.ContainsKey(kel))
            {
                Console.WriteLine(kel + " : " + dic[kel]);
            }
            else
            {
                Console.WriteLine(kel + " tidak ditemukan");
            }
        }

        public void getAllkodebuah()
        {
            foreach (KeyValuePair<string, string> ele1 in dic)
            {
                Console.WriteLine("{0} \t\t {1}", ele1.Key, ele1.Value);
            }
        }
    }


    class PosisiKarakterGame
    {
        enum State { TERBANG, BERDIRI };
        public void jongkok()
        {
            State state = State.TERBANG;

            String[] screenName = { "TERBANG", "BERDIRI" };
            do
            {
                Console.WriteLine("jongkok " + screenName[(int)state]);
                Console.Write("Enter Command : ");
                String command = Console.ReadLine();
                switch (state)
                {
                    case State.TERBANG:
                        if (command == "Posisi Landing")
                        {
                            state = State.BERDIRI;
                        }
                        break;
                    case State.BERDIRI:
                        if (command == "posisi Takeoff")
                        {
                            state = State.TERBANG;
                        }
                        break;



                }
            } while (state != State.TERBANG);
        }
    }


}
