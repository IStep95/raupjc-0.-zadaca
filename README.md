# JMBAG
{ 0036486989 }

# Pitanje 1.
U bin/Debug folder buildane su dvije nove datoteke: ClassLibrary.dll i ClassLibrary.pdb
Nakon što izbrišemo ClassLibrary.dll, KonzolnaAplikacija.exe se ne može pokrenuti.
Program je ispisao: Unhandled Exception: System.IO.FileNotFoundException: Could not load file or assembly 'ClassLibrary, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null' or one of its dependencies. The system cannot find the file specified. at KonzolnaAplikacija.Program.Main(String[] args)
Poslao bih KonzolnaAplikacija.exe i ClassLibrary.dll u jednom folderu.

#Pitanje 2.
Preveo sam samo KonzolnaAplikacija, bez prevođenja ClassLibrary. Aplikacija je prikazala novi string zato jer projekt KonzolnaAplikacija sadrži referencu na projekt ClassLibrary.

#Pitanje 3.
Pero: Hello World

#Pitanje 4.
Bin/Debug folder sad sadrži i PeroClassLibrary.dll

#Pitanje 5.
Ako obrišemo originalni .dll aplikacija i dalje radi. Aplikacija i dalje radi zato jer je sad putanja .dll datoteke u Debug folderu, što može biti vrlo nespretno.

#Pitanje 6.
Aplikacija se uspješno buildala i obrisana datoteka NodaTime 1.3.2. je ponovno stvorena.
