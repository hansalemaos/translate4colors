# automates text translation using Google Translate

## pip install translate4colors 

## Example Usage

```python
textx = r"""Python. was created in the early 1990s by Guido van Rossum at Stichting Mathematisch 
Centrum (CWI, see https://www.cwi.nl/) in the Netherlands as a successor of a 
language called ABC. Guido remains Python’s principal author, although it includes
many contributions from others.

In 1995, Guido. continued his work on Python at the Corporation for 
National Research Initiatives 
(CNRI, see https://www.cnri.reston.va.us/) in Reston, 
Virginia where he released several versions of the software."""

from translate4colors import Gtranslate
with Gtranslate("en", "de") as go:
    data = go.translate(textx)
print(data)

google = Gtranslate("en", "de")
translated = google.translate(textx)
print(translated)
google.quit_translator(soft_kill_first=True)

# [[('Python. was created in the early 1990s by Guido van Rossum at Stichting Mathematisch Centrum (CWI, see https://www.cwi.nl/) in the Netherlands as a successor of a language called ABC. Guido remains Python’s principal author, although it includes many contributions from others. In 1995, Guido. continued his work on Python at the Corporation for National Research Initiatives (CNRI, see https://www.cnri.reston.va.us/) in Reston, Virginia where he released several versions of the software.', 'Python. wurde Anfang der 1990er Jahre von Guido van Rossum am Stichting Mathematisch Centrum (CWI, siehe https://www.cwi.nl/) in den Niederlanden als Nachfolger einer Sprache namens ABC entwickelt. Guido bleibt der Hauptautor von Python, obwohl es viele Beiträge anderer enthält. Im Jahr 1995, Guido. setzte seine Arbeit an Python bei der Corporation for National Research Initiatives (CNRI, siehe https://www.cnri.reston.va.us/) in Reston, Virginia fort, wo er mehrere Versionen der Software veröffentlichte.')]]
# [[('Python. was created in the early 1990s by Guido van Rossum at Stichting Mathematisch Centrum (CWI, see https://www.cwi.nl/) in the Netherlands as a successor of a language called ABC. Guido remains Python’s principal author, although it includes many contributions from others. In 1995, Guido. continued his work on Python at the Corporation for National Research Initiatives (CNRI, see https://www.cnri.reston.va.us/) in Reston, Virginia where he released several versions of the software.', 'Python. wurde Anfang der 1990er Jahre von Guido van Rossum am Stichting Mathematisch Centrum (CWI, siehe https://www.cwi.nl/) in den Niederlanden als Nachfolger einer Sprache namens ABC entwickelt. Guido bleibt der Hauptautor von Python, obwohl es viele Beiträge anderer enthält. Im Jahr 1995, Guido. setzte seine Arbeit an Python bei der Corporation for National Research Initiatives (CNRI, siehe https://www.cnri.reston.va.us/) in Reston, Virginia fort, wo er mehrere Versionen der Software veröffentlichte.')]]
```
