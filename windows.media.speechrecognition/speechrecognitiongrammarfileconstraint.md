---
-api-id: T:Windows.Media.SpeechRecognition.SpeechRecognitionGrammarFileConstraint
-api-type: winrt class
---

<!-- Class syntax.
public class SpeechRecognitionGrammarFileConstraint : Windows.Media.SpeechRecognition.ISpeechRecognitionConstraint, Windows.Media.SpeechRecognition.ISpeechRecognitionGrammarFileConstraint
-->

# Windows.Media.SpeechRecognition.SpeechRecognitionGrammarFileConstraint

## -description
A custom grammar constraint based on a list of words or phrases (defined in a Speech Recognition Grammar Specification (SRGS) file) that can be recognized by the [SpeechRecognizer](speechrecognizer.md) object.

> [!NOTE]
> Speech recognition using a custom constraint is performed on the device.

## -remarks
Constraints, or grammars, define the spoken words and phrases that can be matched by the speech recognizer. You can specify one of the pre-defined, web-service grammars ([SpeechRecognitionTopicConstraint](speechrecognitiontopicconstraint.md)) or you can create a custom grammar, described here, that is installed with your app (speech recognition using a custom constraint is performed on the device).
+ Programmatic list constraints ([SpeechRecognitionListConstraint](speechrecognitionlistconstraint.md)) provide a lightweight approach to creating simple grammars using a list of words or phrases. A list constraint works well for recognizing short, distinct phrases. Explicitly specifying all words in a grammar also improves recognition accuracy, as the speech recognition engine must only process speech to confirm a match. The list can also be programmatically updated.
+ An Speech Recognition Grammar Specification (SRGS) grammar ([SpeechRecognitionGrammarFileConstraint](speechrecognitiongrammarfileconstraint.md)) is a static document that, unlike a programmatic list constraint, uses the XML format defined by the [ Version 1.0](http://go.microsoft.com/fwlink/p/?LinkID=262302). An Speech Recognition Grammar Specification (SRGS) grammar provides the greatest control over the speech recognition experience by letting you capture multiple semantic meanings in a single recognition.

[CompileConstraintsAsync](speechrecognizer_compileconstraintsasync.md) must always be called before [RecognizeAsync](speechrecognizer_recognizeasync.md) or [RecognizeWithUIAsync](speechrecognizer_recognizewithuiasync.md), even if no constraints are specified in the [Constraints](speechrecognizer_constraints.md) property.

## -examples

## -see-also
[Windows.Media.SpeechRecognition](windows_media_speechrecognition.md), [SpeechRecognitionConstraintType](speechrecognitionconstrainttype.md), [ISpeechRecognitionConstraint](ispeechrecognitionconstraint.md), [Speech interactions](http://msdn.microsoft.com/library/646db3ce-fa81-4727-8c21-936c81079439), [Speech design guidelines](http://msdn.microsoft.com/library/4a63a8c4-4182-4e36-ba12-4c343a56fca9), [Speech recognition and speech synthesis sample](http://go.microsoft.com/fwlink/p/?LinkID=619897)