program papatzis;
uses wincrt;
var papas,r:integer;
    logic:char;
    sumE,E:real;

BEGIN

 randomize;
 sumE:=0;
 repeat
  write('posa 8es na pontareis: ');
  read(E);
  writeln('edw papas, ekei papas, pou einai o papas?');
  writeln('epele3e fullo   1    2   3');
  read(papas);

  r:=random(3)+1;  {random einai apo 0 ews 2 opote me to +1 paei apo 1 ws 3}

   if papas=r then
    begin
     writeln('NIKISES!!!');
     sumE:=sumE+E;
     writeln('ta sunolika xrhmata apo ta stoxhmata einai ',sumE:4:2);
    end
   else
    begin
     writeln('EXASES htan sto ',r);
     sumE:=sumE-E;
     writeln('ta sunolika xrhmata apo ta stoixhmata einai ',sumE:4:2);
    end;

   readln;
   writeln('8es allo? y/n');
   read(logic);
   readln;
  until logic='n';

 writeln('na ste kala, na mas 3anar8ete');

 END.
