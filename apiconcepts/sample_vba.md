
# Sample Application in VBA 

Using Visual Basic you can integrate MultiTerm functionality into applications such as Microsoft Office or any other application that supports VBA (Visual Basic for Applications).

To make use of the API, reference the COM component "MultiTerm110.TMO 11.0 Type Library"

The sample code below connects to the local termbase repository, then selects a termbase and performs a search in it.


```vb
Dim oMt As New MultiTermIX.Application
Dim oLocalRep As TermbaseRepository
Dim oTestTermbase As String
oTestTermbase = "C:\Testdata\Sample.sdltb"

'select local termbase repository and log-in
Set oLocalRep = oMt.LocalRepository
oLocalRep.Connect "", ""
  'select termbase
Dim oTbs As Termbases
Set oTbs = oLocalRep.Termbases
oTbs.Add oTestTermbase, "", ""
Dim oTb As Termbase
Set oTb = oTbs.Item(oTestTermbase)

'search termbase
Dim oSearch As TermbaseSearch
Set oSearch = oTb.Search
'configure search parameters
With oSearch
   .Direction = mtSearchDown
   .MaximumHits = 10
   .FuzzySearch = True
   .SearchExpression = "cable"
   .SourceIndex = "English"
End With

'execute search
Dim oHits As HitTerms
Set oHits = oSearch.Execute

'output hit list
Dim oHit As HitTermFor Each oHit In oHits
   Debug.Print oHit.Text
Next
```




