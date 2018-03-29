
# EDataType



##  Attributes
- **serializable** : EBoolean [0..1]

##  Methods

# EPackage



##  Attributes
- **eFactoryInstance** : EFactory [1]
- **eClassifiers** : EClassifier [0..*]
- **eSubpackages** : EPackage [0..*]
- **eSuperPackage** : EPackage [0..1]
- **nsURI** : EString [0..1]
- **nsPrefix** : EString [0..1]

##  Methods
- [**getEClassifier**()](ecore/EPackage/getEClassifier.md)

# EReference



##  Attributes
- **eOpposite** : EReference [0..1]
- **eReferenceType** : EClass [1]
- **eKeys** : EAttribute [0..*]
- **containment** : EBoolean [0..1]
- **container** : EBoolean [0..1]
- **resolveProxies** : EBoolean [0..1]

##  Methods

# EClass



##  Attributes
- **eSuperTypes** : EClass [0..*]
- **eOperations** : EOperation [0..*]
- **eAllAttributes** : EAttribute [0..*]
- **eAllReferences** : EReference [0..*]
- **eReferences** : EReference [0..*]
- **eAttributes** : EAttribute [0..*]
- **eAllContainments** : EReference [0..*]
- **eAllOperations** : EOperation [0..*]
- **eAllStructuralFeatures** : EStructuralFeature [0..*]
- **eAllSuperTypes** : EClass [0..*]
- **eIDAttribute** : EAttribute [0..1]
- **eStructuralFeatures** : EStructuralFeature [0..*]
- **eGenericSuperTypes** : EGenericType [0..*]
- **eAllGenericSuperTypes** : EGenericType [0..*]
- **abstract** : EBoolean [0..1]
- **interface** : EBoolean [0..1]

##  Methods
- [**isSuperTypeOf**()](ecore/EClass/isSuperTypeOf.md)
- [**getFeatureCount**()](ecore/EClass/getFeatureCount.md)
- [**getEStructuralFeature**()](ecore/EClass/getEStructuralFeature.md)
- [**getFeatureID**()](ecore/EClass/getFeatureID.md)
- [**getEStructuralFeature**()](ecore/EClass/getEStructuralFeature.md)

# EEnumLiteral



##  Attributes
- **eEnum** : EEnum [0..1]
- **value** : EInt [0..1]
- **instance** : EEnumerator [0..1]
- **literal** : EString [0..1]

##  Methods

# EAnnotation



##  Attributes
- **eModelElement** : EModelElement [0..1]
- **contents** : EObject [0..*]
- **references** : EObject [0..*]
- **source** : EString [0..1]
- **details** : EStringToStringMapEntry [0..*]

##  Methods

# EStructuralFeature



##  Attributes
- **eContainingClass** : EClass [0..1]
- **changeable** : EBoolean [0..1]
- **volatile** : EBoolean [0..1]
- **transient** : EBoolean [0..1]
- **defaultValueLiteral** : EString [0..1]
- **defaultValue** : EJavaObject [0..1]
- **unsettable** : EBoolean [0..1]
- **derived** : EBoolean [0..1]

##  Methods
- [**getFeatureID**()](ecore/EStructuralFeature/getFeatureID.md)
- [**getContainerClass**()](ecore/EStructuralFeature/getContainerClass.md)

# EEnum



##  Attributes
- **eLiterals** : EEnumLiteral [0..*]

##  Methods
- [**getEEnumLiteral**()](ecore/EEnum/getEEnumLiteral.md)
- [**getEEnumLiteral**()](ecore/EEnum/getEEnumLiteral.md)
- [**getEEnumLiteralByLiteral**()](ecore/EEnum/getEEnumLiteralByLiteral.md)

# ?



##  Attributes

##  Methods

# E



##  Attributes

##  Methods

# ENamedElement



##  Attributes
- **name** : EString [0..1]

##  Methods

# ETypedElement



##  Attributes
- **eType** : EClassifier [0..1]
- **eGenericType** : EGenericType [0..1]
- **ordered** : EBoolean [0..1]
- **unique** : EBoolean [0..1]
- **lowerBound** : EInt [0..1]
- **upperBound** : EInt [0..1]
- **many** : EBoolean [0..1]
- **required** : EBoolean [0..1]

##  Methods

# EFactory



##  Attributes
- **ePackage** : EPackage [1]

##  Methods
- [**create**()](ecore/EFactory/create.md)
- [**createFromString**()](ecore/EFactory/createFromString.md)
- [**convertToString**()](ecore/EFactory/convertToString.md)

# EClassifier



##  Attributes
- **ePackage** : EPackage [0..1]
- **eTypeParameters** : ETypeParameter [0..*]
- **instanceClassName** : EString [0..1]
- **instanceClass** : EJavaClass<?> [0..1]
- **defaultValue** : EJavaObject [0..1]
- **instanceTypeName** : EString [0..1]

##  Methods
- [**isInstance**()](ecore/EClassifier/isInstance.md)
- [**getClassifierID**()](ecore/EClassifier/getClassifierID.md)

# EStringToStringMapEntry



##  Attributes
- **key** : EString [0..1]
- **value** : EString [0..1]

##  Methods

# T



##  Attributes

##  Methods

# EOperation



##  Attributes
- **eContainingClass** : EClass [0..1]
- **eTypeParameters** : ETypeParameter [0..*]
- **eParameters** : EParameter [0..*]
- **eExceptions** : EClassifier [0..*]
- **eGenericExceptions** : EGenericType [0..*]

##  Methods

# E



##  Attributes

##  Methods

# ETypeParameter



##  Attributes
- **eBounds** : EGenericType [0..*]

##  Methods

# EGenericType



##  Attributes
- **eUpperBound** : EGenericType [0..1]
- **eTypeArguments** : EGenericType [0..*]
- **eRawType** : EClassifier [1]
- **eLowerBound** : EGenericType [0..1]
- **eTypeParameter** : ETypeParameter [0..1]
- **eClassifier** : EClassifier [0..1]

##  Methods

# K



##  Attributes

##  Methods

# EModelElement



##  Attributes
- **eAnnotations** : EAnnotation [0..*]

##  Methods
- [**getEAnnotation**()](ecore/EModelElement/getEAnnotation.md)

# EObject



##  Attributes

##  Methods
- [**eClass**()](ecore/EObject/eClass.md)
- [**eIsProxy**()](ecore/EObject/eIsProxy.md)
- [**eResource**()](ecore/EObject/eResource.md)
- [**eContainer**()](ecore/EObject/eContainer.md)
- [**eContainingFeature**()](ecore/EObject/eContainingFeature.md)
- [**eContainmentFeature**()](ecore/EObject/eContainmentFeature.md)
- [**eContents**()](ecore/EObject/eContents.md)
- [**eAllContents**()](ecore/EObject/eAllContents.md)
- [**eCrossReferences**()](ecore/EObject/eCrossReferences.md)
- [**eGet**()](ecore/EObject/eGet.md)
- [**eGet**()](ecore/EObject/eGet.md)
- [**eSet**()](ecore/EObject/eSet.md)
- [**eIsSet**()](ecore/EObject/eIsSet.md)
- [**eUnset**()](ecore/EObject/eUnset.md)

# EParameter



##  Attributes
- **eOperation** : EOperation [0..1]

##  Methods

# EAttribute



##  Attributes
- **eAttributeType** : EDataType [1]
- **iD** : EBoolean [0..1]

##  Methods

# V



##  Attributes

##  Methods

