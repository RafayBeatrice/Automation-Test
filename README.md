# Automation-Test

## **How to log in account**



describe('On OrangeHRM', () => {

      it('I can login', () => {
        cy.visit('https://opensource-demo.orangehrmlive.com/web/index.php/auth/login');
        cy.get(':nth-child(2) > .oxd-input-group > :nth-child(2) > .oxd-input').type('Admin');
        cy.get(':nth-child(3) > .oxd-input-group > :nth-child(2) > .oxd-input').type('admin123');
        cy.get('.oxd-button').click();
    })
})

***************************************************************
## **How to purchase something**

describe('On DemoBlaze', () => {


    
        // it('Purchase', () => {
        //    cy.visit('https://www.demoblaze.com/');
        //    cy.get(':nth-child(1) > .card > .card-block > .card-title > .hrefch').click();
        //     cy.get('.col-sm-12 > .btn').click();
        //     cy.get('#cartur').click();
        //     cy.get('.col-lg-1 > .btn').click();
        //     cy.get('#name').type('test1');
        //     cy.get('#country').type('Romania');
        //     cy.get('#city').type('Brasov');
        //     cy.get('#card').type('123456789');
        //     cy.get('#month').type('3');
        //     cy.get('#year').type('2040');
        //     cy.get('#orderModal > .modal-dialog > .modal-content > .modal-footer > .btn-primary').click();
        //     cy.get('.confirm').click();
        // })


## **How to view "About us "**

        // it('About us', () => {
        //     cy.visit('https://www.demoblaze.com/');
        //     cy.get(':nth-child(3) > .nav-link').click();
        // })
       
    })
