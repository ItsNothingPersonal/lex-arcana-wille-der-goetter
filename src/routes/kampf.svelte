<script>
	import '../app.css';
</script>

<div class="flex flex-col">
	<div class="flex flex-row w-full justify-center">
		<div
			class="prose prose-stone min-w-min font-serif prose-p:leading-relaxed 
			prose-p:text-justify lg:prose-xl prose-figcaption:text-sm 
			prose-figcaption:text-stone-900 prose-blockquote:text-stone-900 
			prose-blockquote:leading-relaxed prose-blockquote:text-justify prose-ul:text-left 
			prose-ol:text-left prose-li:text-justify px-4"
		>
			<section class="container mx-auto text-center py-6 mb-12">
				<h1>Der Kampf</h1>
				<div class="w-full mb-4">
					<div class="h-1 mx-auto bg-white w-1/6 opacity-25 my-0 py-0 rounded-t" />
				</div>
				<p>
					Alle Mitglieder der Cohors Auxiliaria Arca na werden in Kampfkunst ausgebildet, weil -
					Custodes bereit sein müssen, sich allen Gefahren zu stellen, die ihr Leben und ihre
					Mission bedrohen.
				</p>

				<h2>Kampftypen</h2>
				<p>
					Kämpfe sind eine besondere Art von Widerstandsproben mit einigen Spezialregeln. Es gibt
					zwei Grundtypen von Kämpfen: Nahkampf mit Schwertern, Messern, Streitkolben und anderen
					Nahkampfwaffen oder Fernkampf mit Schussoder Wurfwaffen wie Speeren, Schleudern oder
					Bögen. Ein Nahkampf kann entweder ein Duell sein, wenn ein Charakter sich einem einzelnen
					Gegenüber stellen muss, oder ein Charakter tritt gegen mehrere Gegner*innen gleichzeitig
					an.
				</p>

				<h2>Kampfausrüstung</h2>
				<h3>Waffen</h3>
				<p>
					Je nach Typ können Waffen im Nah- oder Fernkampf eingesetzt werden. Manche Waffen können
					mit nur einer Hand geführt werden, für andere benötigt der Charakter beide Hände, um sie
					effektiv einzusetzen. Bei einhändigen Waffen kann gleichzeitig ein Schild getragen werden.
					Spielmechanisch drückt der Schadenswert einer Waffe aus, wie stark sie eine*n Gegner*in
					verwunden kann.
				</p>

				<h3>Rüstung</h3>
				<p>
					Trägt ein Charakter eine Rüstung, kann er den Schaden reduzieren, den ein erfolgreicher
					Angriff der gegnerischen Partei verursacht. Alle Rüstungstypen haben einen Schutzwert
					zwischen 3 und 10, der anzeigt, wieviele Schadenspunkte die Rüstung maximal absorbieren
					kann.
				</p>

				<h3>Schilde</h3>
				<p>
					Schilde verbessern die Chancen eines Charakters, von Angriffen verfehlt zu werden. Ein
					Schild kann nicht zusammen mit einer zweihändigen Waffe eingesetzt werden. Alle Schilde
					haben einen Abwehrwert zwischen 1 und 3, je nachdem, wie groß und stabil sie sind, und
					verbessern damit die Abwehrfähigkeit des Charakters.
				</p>

				<h2>Duelle</h2>
				<p>
					Duelle sind die einfachste Form des Kampfes: zwei Kämpfer*innen bekämpfen sich so lange,
					bis eine*r von beiden sich zurückzieht, aufgibt oder unterliegt. Die Kampfregeln für den
					Kampf gegen mehrere Gegner*innen und mit Fernkampfwaffen werden hier als Varianten eines
					Duells beschrieben.
				</p>

				<h2>Das Tempus</h2>
				<p>
					Wenn es während des Spiels zum Kampf kommt, wird die Zeit in sogenannte Tempora (deutsch:
					Zeitraum, Singular: Tempus) aufgeteilt. Jedes Tempus stellt die Zeit (ein paar Sekunden)
					dar, die benötigt wird, damit beide kämpfenden Charaktere eine Aktion ausführen, einen
					einzelnen Schlagabtausch führen oder einem Angriff ausweichen oder ihn abwehren können.
				</p>

				<h3>Ablauf eines Kampfes</h3>
				<ol>
					<li>
						<b>Auf De Bello würfeln</b><br />
						In jedem Tempus würfeln beide Kämpfenden auf ihren De Bello-Wert und vergleichen die Ergebnisse.
						Wer das höhere Ergebnis erreicht hat, greift in diesem Tempus an, der andere Charakter verteidigt
						sich. Bei Gleichstand hat niemand einen erfolgreichen Schlag ausgeführt und das Tempus wird
						übersprungen.
					</li>
					<li>
						<b>Das AP ausrechnen</b><br />
						Wenn klar ist, welcher Charakter angreift und welcher verteidigt, wird das Angriffspotenzial
						(AP) des angreifenden Charakters berechnet. Dafür wird das De Bello-Würfelergebnis des verteidigenden
						Charakters von dem des angreifenden abgezogen. Trägt der verteidigende Charakter einen Schild,
						wird dessen Abwehrwert ebenfalls vom Würfelergebnis des angreifenden abgezogen. Liegt das
						Angriffspotenzial danach bei null oder weniger, hat der verteidigende Charakter den Schlag
						(mit dem Schild) abgewehrt.
					</li>
					<li>
						<b>Schadensmultiplikator bestimmen</b><br />
						Beträgt das Angriffspotenzial 1 oder mehr, ist dem angreifenden Charakter ein Treffer gelungen.
						Wie viel Schaden der verteidigende Charakter nimmt, hängt vom Schadenswert der Waffe ab,
						der mit einem vom Angriffspotenzial abhängigen Faktor multipliziert wird. Diese Tabelle zeigt,
						welche Faktoren für welche AP-Werte gelten:<br />
						<table>
							<tr><th>AP</th><th>Multiplikator</th></tr>
							<tr><td>1 2 3</td><td>x1</td></tr>
							<tr><td>4 5 6</td><td>x2</td></tr>
							<tr><td>7 8 9</td><td>x3</td></tr>
							<tr><td>10 11 12</td><td>x4</td></tr>
							<tr><td>13 14 15</td><td>x5</td></tr>
							<tr><td>16 oder mehr</td><td>x6</td></tr>
						</table>
					</li>
					<li>
						<b>Schaden auswürfeln</b><br />
						Verursacht ein Charakter Schaden, wählt die Person, die den Charakter führt, den Würfel,
						der der Schadensstufe der benutzten Waffe entspricht, und würfelt ihn so oft, wie der Multiplikator
						vorgibt. Dabei werden alle Ergebnisse zusammengezählt. Für den verteidigenden Charakter wird
						einmal der Würfel geworfen, der seiner Rüstung entspricht. Dann zieht ihr dieses Ergebnis
						vom Gesamtergebnis des vorherigen Schadenswurfes ab. Die Differenz, die danach übrigbleibt,
						entspricht der Anzahl Lebenspunkte, die der verteidigende Charakter verliert.
					</li>
				</ol>

				<p class="border-2 border-stone-400 shadow-2xl p-3 my-4">
					<b>Waffenloser Angriff</b><br />
					Nach den Regeln in diesem Schnellstarter würfelt ein Charakter, der ohne Waffen angreift, normal
					auf De Bello und hat einen Schadenswert von 1. <br />
					In der neuen Version von LEX ARCANA kommt das Pankratium, die römische Kunst des Ring­ und
					Boxkampfes, hinzu, das die Custodes nutzen, um ihre Feind*innen zu unterwerfen, ohne sie zu
					töten.
				</p>

				<h2>Kampf mit mehreren Gegnern</h2>
				<p>
					Eine Kreatur von der Größe eines Menschen kann gleichzeitig von bis zu 3 Gegner*innen
					angegriffen werden, größere Kreaturen sogar von 4 oder mehr. In solchen Fällen wird der
					Kampf behandelt wie mehrere einzelne Duelle, mit ein paar Sonderregeln.
				</p>
				<p>
					Der Hauptunterschied besteht darin, dass der zahlenmäßig unterlegene Charakter sich in
					jedem Tempus der Reihe nach jedem*jeder seiner Gegner*innen stellen muss. Die Reihenfolge
					legt die Partei fest, die zahlenmäßig im Vorteil ist. Die Person, die den unterlegenen
					Charakter führt, würfelt in jedem Tempus einmal De Bello gegen jede*jeden Gegner*in. Diese
					wiederum genießen einen beträchtlichen Vorteil: Für den ersten Angriff würfelt ihr ganz
					normal auf De Bello Alle nachfolgenden Kämpfer*innen zählen das Ergebnis des
					vorausgegangenen Angriffs als Bonus zu ihren Würfelpunkten, bevor sie sich für eine
					Würfelkombination entscheiden.
				</p>

				<h2>Fernkampf</h2>
				<p>
					Fernkampf findet immer dann statt, wenn jemand ein gegnerisches Ziel mit einer
					Fernkampfwaffe angreift, zum Beispiel mit einem Bogen, einem Speer oder einer Schleuder.
					Das Ziel des Angriffs muss sich dafür innerhalb der Reichweite der benutzten Waffe
					befinden. Greifen sich zwei Charaktere gegenseitig mit Fernkampfwaffen an, macht jeder von
					ihnen im gleichen Tempus einen Fernkampfangriff.
				</p>
				<p>
					Die Reichweite legt die Schwierigkeit des Fernkampfangriffs fest. Trägt das Ziel ein
					Schild, wird der Abwehrwert des Schildes zum SG addiert.
				</p>
				<table>
					<tr><th>SG nach Reichweite</th></tr>
					<tr><td>kurz</td><td>3</td><td>ein paar Schritte entfernt bis etwa 10 m</td></tr>
					<tr><td>mittel</td><td>6</td><td>einige dutzend Meter</td></tr>
					<tr><td>weit</td><td>9</td><td>alles darüber hinaus</td></tr>
				</table>
				<p>
					Der Demiurgus kann den SG durch Umstände, wie Deckung, schlechte Sicht oder etwa ein
					bewegtes Zeil noch um jeweils 3 Punkte erhöhen.
				</p>

				<h2>Überraschungsangriffe</h2>
				<p>
					Überraschungsangriffe kommen in LEX ARCANA immer dann vor, wenn ein Charakter nicht merkt,
					dass jemand einen Angriff plant. Ein überraschter Charakter darf sich ein Tempus lang
					nicht gegen den Angriff wehren. Das heißt, das AP eines Überraschungsangriffs entspricht
					genau dem De Bello-Wurf für den angreifenden Charakter. Ab dem darauffolgenden Tempus ist
					dem Opfer des Angriffs die Gefahr voll bewusst und es kann für den Rest des Kampfes normal
					handeln.
				</p>

				<h2>Fliehen</h2>
				<p>
					Wer mit seiner Figur aus einem Kampf fliehen möchte, muss dies am Anfang eines Tempus
					ansagen. Handelt es sich bei dem Kampf um ein Duell, würfelt ihr für beide Charaktere auf
					De Corpore. Ist der Würfelwurf für den fliehenden Charakter höher als der der gegnerischen
					Partei, gelingt die Flucht. Wenn nicht, gilt der Charakter, dessen Fluchtversuch
					scheiterte, einen Tempus lang als überrascht (d.h. Angriffe auf ihn sind Würfelwürfe ohne
					Gegenwehr auf De Bello).
				</p>
				<p>
					Bei mehreren Gegner*innen muss der De Corpore-Wurf für den fliehenden Charakter höher sein
					als alle gegnerischen Würfe.
				</p>

				<h2>Heilen</h2>
				<p>
					Lebenspunkte können auf zwei Arten wieder zurückgewonnen werden: durch die
					<b>natürliche Heilung</b> oder durch <b>Erste Hilfe</b>.
				</p>
				<p>
					Natürliche Heilung passiert automatisch immer dann, wenn ein verwundeter Charakter sich
					längere Zeit ausruht (eine Nacht Schlaf, einen halben Tag Ruhe). Der verwundete Charakter
					heilt Lebenspunkte in Höhe seines Vigor-Wertes.
				</p>
				<p>
					Erste Hilfe kann nur einmal geleistet werden und zwar direkt, nachdem ein Charakter
					verwundet wurde (egal, durch wen oder was). Ein Charakter, der einen anderen oder sich
					selbst heilt, reinigt und verbindet die Wunde oder renkt ein Gelenk oder Körperglied
					wieder ein. Spielmechanisch würfelt die Person, die den Charakter führt, gegen einen SG
					von 6 auf De Scientia. Ist der Wurf erfolgreich, erhält der Charakter die Differenz
					zwischen dem Würfelergebnis und dem Schwierigkeitsgrad in Lebenspunkten zurück. Geht der
					Wurf daneben, erhält er nichts.
				</p>

				<div class="border-2 border-stone-400 shadow-2xl p-3 my-4">
					<h2>Die Sortes</h2>
					<p>
						Zur Standardausrüstung eines Contubernium gehört immer auch ein Beutel, mit einigen
						dünnen, mit Inschriften versehenen Metalltäfelchen darin. Diese Täfelchen nennt man
						Sortes (deutsch: Orakel, Singular: Sors). Sie werden von Mitgliedern des Cohors Arcana
						benutzt, um während einer Mission mehr über ihr Schicksal herauszufinden. Kopiert vor
						Beginn des ersten Abenteuers die in diesem Schnellstarter enthaltenen Sortes, schneidet
						sie aus und legt sie in einen undurchsichtigen Behälter. Wenn ihr zu viert oder weniger
						seid, entfernt die Täfelchen mit den Namen der Custodes, die nicht mitspielen.
					</p>

					<h3>Sortes ziehen</h3>
					<p>
						Die Sortes zu ziehen ist ein kurzes Ritual. Wenn ihr es durchzuführen wollt, teilt ihr
						dem Demiurgus mit, wie viele von euren Charakteren am Ritual teilnehmen. Das Ritual hat
						zwei Voraussetzungen:
					</p>
					<ul>
						<li>Erstens können die Sortes nur einmal pro Spieleabend gezogen werden.</li>
						<li>
							Und zweitens können nur Custodes teilnehmen, die im Verlauf dieses Abenteuers noch
							keine Sors gezogen haben.
						</li>
					</ul>
					<p>
						Jede*r Teilnehmende zieht ein Täfelchen aus dem Beutel, sieht es sich an und legt es
						verdeckt vor sich ab.
					</p>

					<h3>Die Sortes einsetzen</h3>
					<p>
						Jedes Sorstäfelchen beschreibt eine besondere Chance im Spiel, die ihr jederzeit
						einsetzen könnt, solange die beschriebenen Voraussetzungen erfüllt sind. Diese bestehen
						zum Beispiel in der Verwendung einer bestimmten Peritia. Ihr dürft euch euer eigenes
						Täfelchen jederzeit anschauen, aber es ist nicht erlaubt, es den anderen zu zeigen –
						auch nicht dem Demiurgus. Wer dennoch Informationen über seine Sors weitergibt, zieht
						den Zorn der Götter auf seinen Charakter und kann keine Schicksalswürfe mehr machen.
					</p>
					<p>
						Außerdem zieht ihr den Zorn der Götter auf euren Charakter, wenn ihr eure Sors bis zum
						Ende des Spieleabends nicht benutzt habt. Das ist besonders wichtig, weil manche der
						Sortes einen negativen Effekt haben können. In diesem Fall verliert ihr für den
						entsprechenden Charakter für den ganzen nächsten Spielabend die Fähigkeit,
						Schicksalswürfe zu machen. Ausnahme: Das Täfelchen Kein Effekt. Diese Sors wird am Ende
						des Abends einfach abgelegt.
					</p>
				</div>
			</section>
		</div>
	</div>
</div>
