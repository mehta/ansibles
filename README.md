ansibles!
=====

ansible playbook which lamps my work environment.


Usage
-----
Quick availability check

    ansible -i hosts nodename -m ping

Ways to use ansible-command line

to apply all rules (if your ssh-user is a password-less sudoer):

    ansible-playbook -i hosts site.yml

to apply all rules (if doing ssh needs password):

    ansible-playbook -i hosts site.yml --ask-sudo-pass

to apply selective rules (eg. security):

    ansible-playbook -i hosts site.yml -l '&security'

to apply selective rules, to selective node (eg. security/nodeX):

    ansible-playbook -i hosts site.yml -l '&security:nodeX'

Thats all of it! Good to go!


Known Issues
------
Issue: Could not import python modules: apt, apt_pkg. Please install python-apt package.

    ansible -i hosts zeus -a "apt-get install python-apt -y"


Ansible
------

Not sure what Ansible is? Read the getting started here: http://procbits.com/2013/09/08/getting-started-with-ansible-digital-ocean


Future RoadMap
----
- .. nothing yet!

Authors
-------
- **Abhinav Mehta**

License
-------
GPL

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.