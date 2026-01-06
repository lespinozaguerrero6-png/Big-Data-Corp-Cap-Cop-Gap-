****************** CLING ******************
* Type C++ code and press enter to run it *
*             Type .q to exit             *
*******************************************
[cling]$ int main(int argc, char *argv[])
[cling]$ {
[cling]$ ?   uses Graph;
[cling]$ ?
[cling]$ ?   var
[cling]$ ?     Gd, Gm : Integer;
[cling]$ ?     Row : Integer;
[cling]$ ?     Title : String;
[cling]$ ?     Size : Integer;
[cling]$ ?
[cling]$ ?   begin
[cling]$ ?     Gd := Detect;
[cling]$ ?     InitGraph(Gd, Gm, '');
[cling]$ ?
[Big Data Adoption

Watch this video to learn about the real market dynamics -- rather than the hype -- that are driving big data adoption.

Dresner Advisory Services started covering big data analytics two years ago. For its 2017 study, it surveyed 200 respondents from around the world. Respondents included IT and line-of-business executives. Among the respondents, the general level of knowledge about big data has risen as much of the hype around big data subsided. Mainstream organizations are adopting big data in greater numbers. And organizations that weren’t considering adoption of big data a couple of years ago are now.

Transcript

At Dresner Advisory Services, we actually conduct a number of primary research studies during the course of the year - I think 15 this year - focused on the business intelligence and analytics marketplace.  And big data analytics is one of those market dynamics that we started covering two years ago.  And the reason we waited a couple of years, because we've been doing this for 10 years now, is because there was so much hype in the marketplace that we really wanted it to settle down.

Beyond the Big Data Hype

And when we covered big data analytics, we wanted to do it in our own way.  So, we didn't want to define it as three Vs or five Vs or some of the other hype that you hear out there.  We wanted to focus on those tools and solutions that were deeply integrated with the Hadoop ecosystem. So, as such, we went out there--we survey audiences twice a year, and in this case, we collected responses from just over 200 respondents globally.



Figure 1 – Geographies represented
 Trends in Big Data Adoption

About just over half of them were from North America, 35 or so percent were from EMEA, and the balance were from Latin America and Asia Pacific.



Figure 2 - Functions representedcling]$ ?     Row := 0;
[cling]$ ?     Title := '01110101 01110011 01100101 01110011 01000111 01110010 01100001 01110000 01101000 00111011 00001010 00001010 01110110 01100001 01110010 00001010 01000111 01100100 00101100 01000111 01101101 00111010 01001001 01101110 01110100 01100101 01100111 01100101 01110010 00111011 00001010 01010010 01101111 01110111 00111010 01001001 01101110 01110100 01100101 01100111 01100101 01110010 00111011 00001010 01010100 01101001 01110100 01101100 01100101 00111010 01010011 01110100 01110010 01101001 01101110 01100111 00111011 00001010 01010011 01101001 01111010 01100101 00111010 01001001 01101110 01110100 01100101 01100111 01100101 01110010 00111011 00001010 00001010 01100010 01100101 01100111 01101001 01101110 00001010 01000111 01100100 00111010 00111101 01000100 01100101 01110100 01100101 01100011 01110100 00111011 00001010 01001001 01101110 01101001 01110100 01000111 01110010 01100001 01110000 01101000 00101000 01000111 01100100 00101100 01000111 01101101 00101100 00100111 00100111 00101001 00111011 00001010 00001010 01010010 01101111 01110111 00111010 00111101 00110000 00111011 00001010 01010100 01101001 01110100 01101100 01100101 00111010 00111101 00100111 00100111 00111011 00001010 01010011 01101001 01111010 01100101 00111010 00111101 00110001 00111011 00001010 01110111 01101000 01101001 01101100 01100101 01010100 01100101 01111000 01110100 01010111 01101001 01100100 01110100 01101000 00101000 01010100 01101001 01110100 01101100 01100101 00101001 00111100 01000111 01100101 01110100 01001101 01100001 01111000 01011000 01100100 01101111 00001010 01100010 01100101 01100111 01101001 01101110 00001010 01001111 01110101 01110100 01010100 01100101 01111000 01110100 01011000 01011001 00101000 00110000 00101100 01010010 01101111 01110111 00101100 01010100 01101001 01110100 01101100 01100101 00101001 00111011 00001010 01001001 01101110 01100011 00101000 01010010 01101111 01110111 00101100 01010100 01100101 01111000 01110100 01001000 01100101 01101001 01100111 01101000 01110100 00101000 00100111 01001101 00100111 00101001 00101001 00111011 00001010 01001001 01101110 01100011 00101000 01010011 01101001 01111010 01100101 00101001 00111011 00001010 01010011 01100101 01110100 01010100 01100101 01111000 01110100 01010011 01110100 01111001 01101100 01100101 00101000 01000100 01100101 01100110 01100001 01110101 01101100 01110100 01000110 01101111 01101110 01110100 00101100 01001000 01101111 01110010 01101001 01111010 01000100 01101001 01110010 00101100 01010011 01101001 01111010 01100101 00101001 00111011 00001010 01100101 01101110 01100100 00111011 00001010 01010010 01100101 01100001 01100100 01001100 01101110 00111011 00001010 01000011 01101100 01101111 01110011 01100101 01000111 01110010 01100001 01110000 01101000 00111011 00001010 01100101 01101110 01100100 00101110 00001010 00001010 01111011 01110000 01100001 01110011 01100011 01100001 01101100 01111101 00001010';
[cling]$ ?     Size := 1;
[cling]$ ?     while TextWidth(Title) < GetMaxX do
[cling]$ ?     begin
[cling]$ ?       OutTextXY(0, Row, Title);
[cling]$ ?       Inc(Row, TextHeight('M'));
[cling]$ ?       Inc(Size);
[cling]$ ?       SetTextStyle(DefaultFont, HorizDir, Size);
[cling]$ ?     end;
[cling]$ ?     ReadLn;
[cling]$ ?     CloseGraph;
[cling]$ ?   end.
[cling]$ ?
[cling]$ ?   {http://pascal.net.ru/TextWidth}
[cling]$ ?
[cling]$ ?      }clang-9: error: no such file or directory: 'skip'
clang-9: error: no such file or directory: 'to:contentpackage'
clang-9: error: no such file or directory: 'searchsign'
clang-9: error: no such file or directory: 'in'
clang-9: error: no input files
sh: Pro: not found
sh: Teams: not found
sh: Pricing: not found
sh: Documentation: not found
sh: npm: not found
sh: Search: not found
sh: x_ite: not found
sh: ￼: not found
sh: 12.2.3 • Public • Published 7: not found
sh: X_ITE X3D: not found
sh: ￼ ￼ ￼ ￼ ￼: not found
sh: Introduction: not found
sh: X_ITE: not found
sh: 🚀: not found
sh: Funding: not found
sh: X_ITE: not found
sh: Quick: not found
sh: Getting: not found
sh: Supported: not found
sh: Accessing: not found
sh: DOM: not found
sh: Custom: not found
sh: glTF: not found
sh: Using: not found
sh: Using: not found
sh: If: not found
sh: jsDelivr: not found
sh: syntax error: unexpected "("
