JFLAGS =
JC = javac
.SUFFIXES: .java .class
.java.class:
		$(JC) $(JFLAGS) $*.java

CLASSES = \
		Main.java \
		codeGenerator/AbstractAssemblyCodePrinter.java \
		codeGenerator/AbstractCodeGenerator.java \
		codeGenerator/AbstractExpressionParser.java \
		codeGenerator/codeGenerator/CodeGenerator.java \
		codeGenerator/codeGenerator/ExpressionParser.java \
		codeGenerator/optimizedCodeGenerator/OptimizedCodeGenerator.java \
		codeGenerator/optimizedCodeGenerator/OptimizedExpressionParser.java \
		codeGenerator/optimizedCodeGenerator/RegisterPool.java \
		codeGenerator/utilities/DeclarationMangler.java \
		codeGenerator/utilities/Instruction.java \
		codeGenerator/utilities/Register.java \
		driver/Driver.java \
		exception/Exception.java \
		exception/ExceptionHandler.java \
		exception/ExceptionStrength.java \
		exception/IException.java \
		interpreter/Environment.java \
		interpreter/Interpreter.java \
		interpreter/boxes/ArrayBox.java \
		interpreter/boxes/Box.java \
		interpreter/boxes/IntegerBox.java \
		interpreter/boxes/RecordBox.java \
		parser/Parser.java \
		parser/semanticAnalysis/SemanticValidator.java \
		parser/semanticAnalysis/abstractSyntaxTree/Node.java \
		parser/semanticAnalysis/abstractSyntaxTree/conditions/Condition.java \
		parser/semanticAnalysis/abstractSyntaxTree/conditions/relation/IRelation.java \
		parser/semanticAnalysis/abstractSyntaxTree/conditions/relation/Relation.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/Binary.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/Expression.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/Function.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/InvalidExpression.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/Number.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/Operator.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/Field.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/Index.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/InvalidLocation.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/InvalidVariable.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/Location.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/Variable.java \
		parser/semanticAnalysis/abstractSyntaxTree/expressions/utilities/ConstantFolder.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Assign.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Call.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/If.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Instruction.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Read.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Repeat.java \
		parser/semanticAnalysis/abstractSyntaxTree/instructions/Write.java \
		parser/semanticAnalysis/abstractSyntaxTree/printers/AbstractSyntaxTreeDotSyntaxPrinter.java \
		parser/semanticAnalysis/abstractSyntaxTree/printers/AbstractSyntaxTreePrinter.java \
		parser/semanticAnalysis/abstractSyntaxTree/printers/IAbstractSyntaxTreePrinter.java \
		parser/semanticAnalysis/symbolTable/declarations/Declaration.java \
		parser/semanticAnalysis/symbolTable/declarations/DeclarationBuilder.java \
		parser/semanticAnalysis/symbolTable/declarations/InvalidDeclaration.java \
		parser/semanticAnalysis/symbolTable/declarations/constants/constant/Constant.java \
		parser/semanticAnalysis/symbolTable/declarations/constants/constant/ConstantBuilder.java \
		parser/semanticAnalysis/symbolTable/declarations/constants/constant/InvalidConstant.java \
		parser/semanticAnalysis/symbolTable/declarations/procedures/Argument.java \
		parser/semanticAnalysis/symbolTable/declarations/procedures/LocalVariable.java \
		parser/semanticAnalysis/symbolTable/declarations/procedures/Parameter.java \
		parser/semanticAnalysis/symbolTable/declarations/procedures/Procedure.java \
		parser/semanticAnalysis/symbolTable/declarations/procedures/ProcedureBuilder.java \
		parser/semanticAnalysis/symbolTable/declarations/types/Integer.java \
		parser/semanticAnalysis/symbolTable/declarations/types/InvalidType.java \
		parser/semanticAnalysis/symbolTable/declarations/types/Type.java \
		parser/semanticAnalysis/symbolTable/declarations/types/Void.java \
		parser/semanticAnalysis/symbolTable/declarations/types/array/Array.java \
		parser/semanticAnalysis/symbolTable/declarations/types/array/ArrayBuilder.java \
		parser/semanticAnalysis/symbolTable/declarations/types/array/InvalidArray.java \
		parser/semanticAnalysis/symbolTable/declarations/types/record/InvalidRecord.java \
		parser/semanticAnalysis/symbolTable/declarations/types/record/Record.java \
		parser/semanticAnalysis/symbolTable/declarations/types/record/RecordBuilder.java \
		parser/semanticAnalysis/symbolTable/declarations/variable/InvalidVariable.java \
		parser/semanticAnalysis/symbolTable/declarations/variable/Variable.java \
		parser/semanticAnalysis/symbolTable/declarations/variable/VariableBuilder.java \
		parser/semanticAnalysis/symbolTable/printers/ISymbolTablePrinter.java \
		parser/semanticAnalysis/symbolTable/printers/SymbolTableDotSyntaxPrinter.java \
		parser/semanticAnalysis/symbolTable/printers/SymbolTablePrinter.java \
		parser/semanticAnalysis/symbolTable/scope/Scope.java \
		parser/semanticAnalysis/symbolTable/scope/ScopeManager.java \
		parser/syntacticAnalysis/ProductionRule.java \
		parser/syntacticAnalysis/SyntacticExceptionHandler.java \
		parser/syntacticAnalysis/SyntacticSynchronizationCoordinator.java \
		parser/syntacticAnalysis/SyntacticValidator.java \
		parser/syntacticAnalysis/events/ParserEvent.java \
		parser/syntacticAnalysis/events/dispatcher/IParserEventDispatcher.java \
		parser/syntacticAnalysis/events/dispatcher/ParserEventDispatcher.java \
		parser/syntacticAnalysis/events/listeners/IParserEventListener.java \
		parser/syntacticAnalysis/printers/IParseTreePrinter.java \
		parser/syntacticAnalysis/printers/ParseTreeDotSyntaxPrinter.java \
		parser/syntacticAnalysis/printers/ParseTreePrinter.java \
		parser/utilities/DesignatorType.java \
		parser/utilities/ExpressionParser.java \
		parser/utilities/TokenIterator.java \
		parser/utilities/Tuple.java \
		scanner/Scanner.java \
		scanner/utilities/BufferedInputReader.java \
		scanner/utilities/CharacterIterator.java \
		scanner/utilities/CharacterUtilities.java \
		shared/InvalidToken.java \
		shared/Reserved.java \
		shared/Token.java \
		shared/utilities/iterator/AbstractIterator.java \
		shared/utilities/iterator/Iterator.java \

default: classes

classes: $(CLASSES:.java=.class)

clean:
		$(RM) *.class
		$(RM) codeGenerator/*.class
		$(RM) driver/*.class
		$(RM) exception/*.class
		$(RM) interpreter/*.class
		$(RM) parser/*.class
		$(RM) scanner/*.class
		$(RM) shared/*.class
		$(RM) codeGenerator/codeGenerator/*.class
		$(RM) codeGenerator/optimizedCodeGenerator/*.class
		$(RM) codeGenerator/utilities/*.class
		$(RM) interpreter/boxes/*.class
		$(RM) parser/semanticAnalysis/*.class
		$(RM) parser/syntacticAnalysis/*.class
		$(RM) parser/utilities/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/*.class
		$(RM) parser/semanticAnalysis/symbolTable/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/conditions/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/expressions/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/instructions/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/printers/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/conditions/relation/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/expressions/locations/*.class
		$(RM) parser/semanticAnalysis/abstractSyntaxTree/expressions/utilities/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/*.class
		$(RM) parser/semanticAnalysis/symbolTable/printers/*.class
		$(RM) parser/semanticAnalysis/symbolTable/scope/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/constants/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/procedures/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/types/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/variable/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/constants/constant/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/types/array/*.class
		$(RM) parser/semanticAnalysis/symbolTable/declarations/types/record/*.class
		$(RM) parser/syntacticAnalysis/events/*.class
		$(RM) parser/syntacticAnalysis/printers/*.class
		$(RM) parser/syntacticAnalysis/events/dispatcher/*.class
		$(RM) parser/syntacticAnalysis/events/listeners/*.class
		$(RM) scanner/utilities/*.class
		$(RM) shared/utilities/*.class
		$(RM) shared/utilities/iterator/*.class
