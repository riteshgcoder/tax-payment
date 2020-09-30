'''
1. create person class and set tax amount
2. derive businessman and employee classes
- set other tax amount on them '''
class person:
    def__init__(self,id_number):
        self.id_number=id_number
    def pay_tax(self,taxable_income,tax_rate):
        tax=taxable_income*tax_rate
        print('the tax is $' + str(tax))
        return tax
class businessman(person):
    def pay_tax(self,taxable_income,business_allowance,tax_rate):
        tax=(taxable_income-business_allowance)*tax_rate
        print('The tax is $'+str(tax))
        return tax
class employee(person):
    def refund_tax(self,amount):
        print('The refund is $'+str(amount))
        return amount
rohan_businessman=businessman('A123445')
rohan_tax=tax_businessman.pay_tax(60000,600,0.8)

ram_self_employed=person('T88679')
rohan_tax=ram_self_employed.pay_tax(633937,0.45)

ayush_employee=employee('k233536')
ayush_tax=ayush_employee.pay_tax(363383,0.73)
ayush_refund=ayush_employee.refund_tax(3637)
